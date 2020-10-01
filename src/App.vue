<template>
<Header title="Neal.fun" />
<Box msg="Spend Bill Gates' Money" />
<MoneyLine money="$100,000,000,000" />
<div class="container">
    <CardProduct v-for="product in products" :key="product" :image="product.image" :sku="product.sku" :price="product.price" :initialValue="product.initialValue" :id="product.id" />
</div>
</template>

<script>
import Header from "./components/Header/Header";
import Box from "./components/Box/Box";
import MoneyLine from "./components/MoneyLine/MoneyLine"
import CardProduct from './components/CardProduct/CardProduct'

import BigMac from './assets/big-mac.jpg'
import FlipFlops from './assets/flip-flops.jpg'
import CocacolaPakc from './assets/coca-cola-pack.jpg'
import MovieTicket from './assets/movie-ticket.jpg'
import Book from './assets/book.jpg'
import Lobster from './assets/lobster-dinner.jpg'
import VideoGame from './assets/video-game.jpg'
import AmazonEcho from './assets/amazon-echo.jpg'
import Netflix from './assets/year-of-netflix.jpg'
import Jordans from './assets/air-jordans.jpg'
import AirPods from './assets/airpods.jpg'
import GameConsole from './assets/gaming-console.jpg'
import Drone from './assets/drone.jpg'
import Smarthphone from './assets/smartphone.jpg'
import Bike from './assets/bike.jpg'
import Kitten from './assets/kitten.jpg'
import Puppy from './assets/puppy.jpg'
import AutoRickshaw from './assets/auto-rickshaw.jpg'
import Horse from './assets/horse.jpg'
import AcreOfFarmland from './assets/acre-of-farmland.jpg'
import DesignerHandbag from './assets/designer-handbag.jpg'
import Hotub from './assets/hot-tub.jpg'
import LuxuryWine from './assets/luxury-wine.jpg'
import DiamondRing from './assets/diamond-ring.jpg'
import JetSki from './assets/jet-ski.jpg'
import Rolex from './assets/rolex.jpg'
import Ford150 from './assets/ford-f-150.jpg'
import Tesla from './assets/tesla.jpg'
import MonsterTruck from './assets/monster-truck.jpg'
import Ferrari from './assets/ferrari.jpg'
import SingleFamilyHome from './assets/single-family-home.jpg'
import GoldBar from './assets/gold-bar.jpg'
import McDonaldsFranchise from './assets/mcdonalds-franchise.jpg'
import SuperbowlAd from './assets/superbowl-ad.jpg'
import Yacht from './assets/yacht.jpg'
import Tank from './assets/m1-abrams.jpg'
import Formula1Car from './assets/formula-1-car.jpg'
import ApacheHelicopter from './assets/apache-helicopter.jpg'
import Mansion from './assets/mansion.jpg'
import MakeaMovie from './assets/make-a-movie.jpg'
import Boeing747 from './assets/boeing-747.jpg'
import MonaLisa from './assets/mona-lisa.jpg'
import Skyscraper from './assets/skyscraper.jpg'
import CruiseShip from './assets/cruise-ship.jpg'
import NBATeam from './assets/nba-team.jpg'

let products = [{
        "id": 1,
        "image": BigMac,
        "sku": "Big Mac",
        "price": "$2",
        "initialValue": "0"
    },
    {
        "id": 2,
        "image": FlipFlops,
        "sku": "Flip Flops",
        "price": "$3",
        "initialValue": "0"
    },
    {
        "id": 3,
        "image": CocacolaPakc,
        "sku": "Coca-Cola Pack",
        "price": "$5",
        "initialValue": "0"
    },
    {
        "id": 4,
        "image": MovieTicket,
        "sku": "Movie Ticket",
        "price": "$12",
        "initialValue": "0"
    },
    {
        "id": 5,
        "image": Book,
        "sku": "Book",
        "price": "$15",
        "initialValue": "0"
    },
    {
        "id": 6,
        "image": Lobster,
        "sku": "Lobster Dinner",
        "price": "$45",
        "initialValue": "0"
    },
    {
        "id": 7,
        "image": VideoGame,
        "sku": "Video Game",
        "price": "$60",
        "initialValue": "0"
    },
    {
        "id": 8,
        "image": AmazonEcho,
        "sku": "Amazon Echo",
        "price": "$99",
        "initialValue": "0"
    },
    {
        "id": 9,
        "image": Netflix,
        "sku": "Year of Netflix",
        "price": "$100",
        "initialValue": "0"
    },
    {
        "id": 10,
        "image": Jordans,
        "sku": "Air Jordans",
        "price": "$125",
        "initialValue": "0"
    },
    {
        "id": 11,
        "image": AirPods,
        "sku": "Airpods",
        "price": "$199",
        "initialValue": "0"
    },
    {
        "id": 12,
        "image": GameConsole,
        "sku": "Gaming Console",
        "price": "$299",
        "initialValue": "0"
    },
    {
        "id": 13,
        "image": Drone,
        "sku": "Drone",
        "price": "$350",
        "initialValue": "0"
    },
    {
        "id": 14,
        "image": Smarthphone,
        "sku": "Smartphone",
        "price": "$699",
        "initialValue": "0"
    },
    {
        "id": 15,
        "image": Bike,
        "sku": "Bike",
        "price": "$800",
        "initialValue": "0"
    },
    {
        "id": 16,
        "image": Kitten,
        "sku": "Kitten",
        "price": "$1,500",
        "initialValue": "0"
    },
    {
        "id": 17,
        "image": Puppy,
        "sku": "Puppy",
        "price": "$1,500",
        "initialValue": "0"
    },
    {
        "id": 18,
        "image": AutoRickshaw,
        "sku": "Auto Rickshaw",
        "price": "$2,300",
        "initialValue": "0"
    },
    {
        "id": 19,
        "image": Horse,
        "sku": "Horse",
        "price": "$2,500",
        "initialValue": "0"
    },
    {
        "id": 20,
        "image": AcreOfFarmland,
        "sku": "Acre of Farmland",
        "price": "$3,000",
        "initialValue": "0"
    },
    {
        "id": 21,
        "image": DesignerHandbag,
        "sku": "Designer Handbag",
        "price": "$5,500",
        "initialValue": "0"
    },
    {
        "id": 22,
        "image": Hotub,
        "sku": "Hot Tub",
        "price": "$6,000",
        "initialValue": "0"
    },
    {
        "id": 23,
        "image": LuxuryWine,
        "sku": "Luxury Wine",
        "price": "$7,000",
        "initialValue": "0"
    },
    {
        "id": 24,
        "image": DiamondRing,
        "sku": "Diamond Ring",
        "price": "$10,000",
        "initialValue": "0"
    },
    {
        "id": 25,
        "image": JetSki,
        "sku": "Jet Ski",
        "price": "$12,000",
        "initialValue": "0"
    },
    {
        "id": 26,
        "image": Rolex,
        "sku": "Rolex",
        "price": "$15,000",
        "initialValue": "0"
    },
    {
        "id": 27,
        "image": Ford150,
        "sku": "Ford F-150",
        "price": "$30,000",
        "initialValue": "0"
    },
    {
        "id": 28,
        "image": Tesla,
        "sku": "Tesla",
        "price": "$75,000",
        "initialValue": "0"
    },
    {
        "id": 29,
        "image": MonsterTruck,
        "sku": "Monster Truck",
        "price": "$150,000",
        "initialValue": "0"
    },
    {
        "id": 30,
        "image": Ferrari,
        "sku": "Ferrari",
        "price": "$250,000",
        "initialValue": "0"
    },
    {
        "id": 31,
        "image": SingleFamilyHome,
        "sku": "Single Family Home",
        "price": "$300,000",
        "initialValue": "0"
    },
    {
        "id": 32,
        "image": GoldBar,
        "sku": "Gold Bar",
        "price": "$700,000",
        "initialValue": "0"
    },
    {
        "id": 33,
        "image": McDonaldsFranchise,
        "sku": "McDonalds Franchise",
        "price": "$1,500,000",
        "initialValue": "0"
    },
    {
        "id": 34,
        "image": SuperbowlAd,
        "sku": "Superbowl Ad",
        "price": "$5,250,000",
        "initialValue": "0"
    },
    {
        "id": 35,
        "image": Yacht,
        "sku": "Yacht",
        "price": "$7,500,000",
        "initialValue": "0"
    },
    {
        "id": 36,
        "image": Tank,
        "sku": "M1 Abrams",
        "price": "$8,000,000",
        "initialValue": "0"
    },
    {
        "id": 37,
        "image": Formula1Car,
        "sku": "Formula 1 Car",
        "price": "$15,000,000",
        "initialValue": "0"
    },
    {
        "id": 38,
        "image": ApacheHelicopter,
        "sku": "Apache Helicopter",
        "price": "$31,000,000",
        "initialValue": "0"
    },
    {
        "id": 39,
        "image": Mansion,
        "sku": "Mansion",
        "price": "$45,000,000",
        "initialValue": "0"
    },
    {
        "id": 40,
        "image": MakeaMovie,
        "sku": "Make a Movie",
        "price": "$100,000,000",
        "initialValue": "0"
    },
    {
        "id": 41,
        "image": Boeing747,
        "sku": "Boeing 747",
        "price": "$148,000,000",
        "initialValue": "0"
    },
    {
        "id": 42,
        "image": MonaLisa,
        "sku": "Mona Lisa",
        "price": "$780,000,000",
        "initialValue": "0"
    },
    {
        "id": 43,
        "image": Skyscraper,
        "sku": "Skyscraper",
        "price": "$850,000,000",
        "initialValue": "0"
    },
    {
        "id": 44,
        "image": CruiseShip,
        "sku": "Cruise Ship",
        "price": "$930,000,000",
        "initialValue": "0"
    },
    {
        "id": 45,
        "image": NBATeam,
        "sku": "NBA Team",
        "price": "$2,120,000,000",
        "initialValue": "0"
    }

]
export default {
    name: "App",
    data: function () {
        return {
            products: products
        };
    },
    components: {
        Header,
        Box,
        MoneyLine,
        CardProduct
    },
    computed: {
        computedProducts(products) {
            return products
        }
    }
};
</script>

<style lang="scss">
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}

body {
    background-color: #f1f2f6;
}

.container {
    display: grid;
    grid-template-columns: repeat(3, minmax(0px, 1fr));
    gap: 10px;
    margin: 0 auto;
    max-width: 1000px;
}
</style>
