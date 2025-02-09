// Définition de l'interface Véhicule
interface Vehicule {
    make: string;
    model: string;
    year: number;
    start(): void;
}

class Voiture implements Vehicule {
    make: string;
    model: string;
    year: number;

    constructor(make: string, model: string, year: number) {
        this.make = make;
        this.model = model;
        this.year = year;
    }

    start(): void {
        console.log("Car engine started");
    }
}

const maVoiture = new Voiture("Toyota", "Corolla", 2022);

maVoiture.start();
