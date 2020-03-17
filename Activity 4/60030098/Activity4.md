4.เขียนเรื่องจาก Keyword ที่กำหนดให้ดังต่อไปนี้

Encapsulation

Inheritance

Polymorphism

**Encapsulation**

คือ คุณสมบัติการห่อหุ้ม หรือการกำหนดการเข้าถึงคุณสมบัติและพฤติกรรมของคลาสซึ่งประกอบไปด้วย

    1.Private สามารถเข้าถึงได้ในเฉพาะคลาสของตนเอง

    2.Protected สามารถเข้าถึงได้เฉพาะคลาสตัวเองและคลาสที่สืบทอดไปเท่านั้น

    3.Public เป็นคลาสที่สามารถเข้าถึงจากคลาสใดๆก็ได้

**Inheritance**

คือ คุณสมบัติการสืบทอด โดยที่คลาสหลักสามารถสืบทอดคุณสมบัติของตนเองให้กับคลาสที่เป็นคลาสย่อยได้ ยกตัวอย่างเช่น

```java
public class InheritanceExample {
    public static void main (String[] args) {
        Artist art = new Artist("Marcus", 20);
        Athlete ath = new Athlete("Danny", 25);

        art.genre = "Trip Hop";
        ath.sport = "Football";

        art.introduce();
        art.playMusic();

        System.out.println();

        ath.introduce();
        ath.playSport();
    }
}

class Person {
    String name;
    int age;

    public Person () {
    }

    public Person (String name, int age) {
        this.name = name;
        this.age = age;
    }

    public void introduce () {
        System.out.println("My name is " + name);
    }
}

class Artist extends Person {
    String genre;

    public Artist (String name, int age){
        this.name = name;
        this.age = age;
    }

    public void playMusic () {
        System.out.println(name + " is playing " + genre + " music.");
    }
}

class Athlete extends Person {
    String sport;

    public Athlete (String name, int age){
        this.name = name;
        this.age = age;
    }

    public void playSport () {
        System.out.println(name + " is playing " + sport + ".");
    }
}
```

**Polymorphism**
คือ คุณสมบัติที่จะสามารถทำให้ Object มีได้หลากหลายรูปแบบ ยกตัวอย่างเช่น

```java
public class TestPolymorphism {

    public static void main (String[] args) {

        Person person1, person2, person3;
        person1 = new Person("Mark", 1980);
        person2 = new Sheriff("Mateo", 1981, "California");
        person3 = new Police("Danny", 1986, "NYC");

        person1.introduce();
        person2.introduce();
        person3.introduce(); 

    }  

}

class Person {

    String name;
    int bornYear;

    public Person (String name, int bornYear) {
        this.name = name;
        this.bornYear = bornYear;
    }

    public void introduce () {
        System.out.print("My name is " + name + ",");
        System.out.println(" I was born in " + bornYear + ".");
    }

}

class Sheriff extends Person {

    String workState;

    public Sheriff (String name, int bornYear, String workState) {
        super(name, bornYear);
        this.workState = workState;
    }

    @Override
    public void introduce () {
        super.introduce();
        System.out.println("I'm a sheriff and work in " + 
                workState + ".");
    }

}

class Police extends Person {

    String workCountry;

    public Police (String name, int bornYear, String workCountry) {
        super(name, bornYear);
        this.workCountry = workCountry;
    }

    @Override
    public void introduce () {
        super.introduce();
        System.out.println("I'm a police and work in " + 
                workCountry + ".");
    }

}
```

อ้างอิงจาก http://marcuscode.com/lang/java/polymorphism