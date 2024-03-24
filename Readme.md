```js
class Vehicle {
    constructor(color = "blue", numberOfWheels = 4, horn = "beep beep") {
        this.color = color;
        this.numberOfWheels = numberOfWheels;
        this.horn = horn;
    }

    honkHorn()
    {
        console.log(this.horn);
    }
}

class Bicycle extends Vehicle{
    constructor(color = "blue", numberOfWheels = 2, horn = "honk honk") {
        super(color,numberOfWheels,horn);
    }
}

let obj = new Bicycle();

console.log(obj.color);
console.log(obj.numberOfWheels);
console.log(obj.horn);
obj.honkHorn();
```