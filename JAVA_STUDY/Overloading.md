# 오버로딩(Overloading)
## 정의

<aside>
💡 같은 이름이지만 서로 다른 매개변수의 형식으로 여러개로 정의하는 방법. 즉, 동일한 이름이지만 다른 기능을 하는 메서드를 말한다.

</aside>

---

## 사용법

기존에 받는 매개변수의 수를 변경 → 기존에 존재했던 매개변수의 숫자 만큼을 입력하지 못하기 때문에 오류 발생

- **메서드 이름 변경**

```java
A.set2(1, 2);
A.set3(1, 2, 3);
```

- **기존 클래스 형식**

```java
class calcul {
int a, b,;
int c = 0;

public void set(int a, int b){
this.a = a;
this.b = b;
}

public void set(int a, int b, int c) {
this.a = a;
this.b = b; // 중복이므로 this.set(a, b)를 사용하여 중복을 제거할 수 있다.
this.c = c;
}
}
```

⭐ 메서드명이 같아도 받는 매개변수의 수가 다르기 때문에 다른 메서드로 인식한다. 따라서 오류가 발생하지 않는다.

---

## 오버라이딩 vs 오버로딩

- 메서드를 여러가지 방법으로 사용

> 궁극적으로, 오버라이딩은 부모 클래스를 상속받은 자식클래스가 자식클래스만의 **새로운 기능을 추가하거나 동작 방법을 변경**하는 것이다. 오버로딩은 **같은 이름, 다른 매개변수의 메서드들을 여러개 만들 수 있다**는 의미이다.
>