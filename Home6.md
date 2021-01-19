package org.geekbrein;

public class Main2 {
    public static void main(String[] args) {
        Dog dog = new Dog("Черный",9,"Бобик", 500,10);
        Cat cat = new Cat("Белый",11,"Дуська",200,0);
        System.out.println("Цвет кошки:" + cat.getColor() + ". Возвраст:" + cat.getAge() + ". Имя: " + cat.getnName() + ". Бег:" + cat.getRun() + ". Дуська проплывет:" + cat.getSwimming());
        System.out.println("Цвет собаки:" + dog.getColor() + ". Возвраст:" + dog.getAge() + ". Имя: " + dog.getnName() + ". Бег:" + dog.getRun() + ". Бобиг проплывает:" + dog.getSwimming());
    }
}
 
//Animal
package org.geekbrein;

public class Animal {
    private String color;
    private int age;
    private String name;
    public int run;
    private int swimming;

    public Animal(String color, int age, String name, int run, int swimming) {
        this.color = color;
        this.age = age;
        this.name = name;
        this.run = run;
        this.swimming = swimming;
    }

    public String getColor() {
        return color;
    }

    public void setColor(String color) {
        this.color = color;
    }

    public int getAge() {
         return age;
    }
    public void setAge(int age) {
        this.age = age;
    }


    public String getnName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }

    public int getRun() {
        return run;
    }

    public void setRun(int swimming) {
        this.swimming = swimming;
    }
    public int getSwimming() {
        return swimming;
    }

    public void setSwimming(int swimming) {
        this.swimming = swimming;
    }
}

//Cat
package org.geekbrein;

import javax.xml.namespace.QName;

public class Cat extends Animal {


    public Cat(String color, int age, String name, int run, int swimming) {
        super(color, age, name, run, swimming);
    }
}

//Dog
package org.geekbrein;

public class Dog extends Animal {


    public Dog(String color, int age, String name, int run, int swimming) {
        super(color, age, name, run, swimming);
    }
}
