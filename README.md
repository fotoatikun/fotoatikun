<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body class="">
    
    <div class="container">
        <header>
            <h1>Your Shopping Cart</h1>
            <div class="shopping">
                <img src="imgs/hi.jpg">
                <span class="quantity">0</span>
            </div>
        </header>

        <div class="list">
          
        </div>
    </div>
    <div class="card">
        <h1>Card</h1>
        <ul class="listCard">
        </ul>
        <div class="checkOut">
            <div class="total">0</div>
            <div class="closeShopping">Close</div>
        </div>
    </div>
    <div class="bg">
        <ul class="glass">
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
        </ul>

    <script src="app.js"></script>
</body>
  </html>
#-----------------now css---------------------------------------------
  body{
    background-color: #E3E7E8;
    font-family: system-ui;
}
.container{
    width: 1000px;
    margin: auto;
    transition: 0.5s;
}
header{
    display: grid;
    grid-template-columns: 1fr 50px;
    margin-top: 50px;
}
header .shopping{
    position: relative;
    text-align: right;
}
header .shopping img{
    width: 40px;
}
header .shopping span{
    background: red;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #fff;
    position: absolute;
    top: -5px;
    left: 80%;
    padding: 3px 10px;
}
.list{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    column-gap: 20px;
    row-gap: 20px;
    margin-top: 50px;
}
.list .item{
    text-align: center;
    background-color: #DCE0E1;
    padding: 20px;
    box-shadow: 0 50px 50px #757676;
    letter-spacing: 1px;
}
.list .item img{
    width: 90%;
}
.list .item .title{
    font-weight: 600;
}
.list .item .price{
    margin: 10px;
}
.list .item button{
    background-color: #1C1F25;
    color: #fff;
    width: 100%;
    padding: 10px;
}
.card{
    position: fixed;
    top:0;
    left: 100%;
    width: 500px;
    background-image: url(data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxANDg0NDQ0NDQ0NDQ0NDQ0NDQ8NDQ0NFREWFhURExMYHSggGBolGxMTITEhMSk3Oi4uFx8zODMtNygtLisBCgoKDg0OFw8PFysZFRkrKy0rKystLTctKysrLSs3LS0tLS0tKy0rLSstNy0tLTctLSstLS0rKysrKy0rLS0tK//AABEIAKgBLAMBIgACEQEDEQH/xAAaAAADAQEBAQAAAAAAAAAAAAABAgMABAUG/8QAIBABAQEAAwEBAAIDAAAAAAAAAAECAxESIRMxQQRhgf/EABwBAAMBAQEBAQEAAAAAAAAAAAIDBAEABQcGCP/EABsRAQEBAQEBAQEAAAAAAAAAAAABAhEDIRIx/9oADAMBAAIRAxEAPwD5uwtVsJY+gSvxsqOonV7E9ZHKZKnSai1hbGjlQ1Ed5dOoS5DYbnTkuU9x13Ce8FaybnTj1kvTpuSawRrCnGksRWZNjCkyX+T5UfDeVaUjcirzhZGuDSHzlLtd5xLwbOVpgfJGopxEfIzKnk3n4n1FWYlIduhhG6oxkZA3g0UmSNKc56Tj41ZxK4x8NIXxTnEkQvGE4HT0PQbBzEc/49HzxrTJ5hnBzDluG8OqYN+buN/DmznprItvKOsuZZxHUDytMj4YH8u7UL5X1lPUfQZXxKVGwth7A6MlHKlYFitgXLei657kPK1jeGj/AE5tZQ5HbrCG+NlhuNOK0q28Euek+otxWzGtaATqqsQS02YpOPtNuWrfPkTxl0Y41OPi6V8l3zV4059TovS24luEbzxTikNSU2UHpV3nC9HzB6PmJqrzGkUzlpD5BYfk+B0XEDloeHd+F1s+ahf5WwCuzVcqZpcztSZCfD5ybyWXo800xLly59Orl+ufyyg1CTJ5k+MqeXcdMujSHIfdQ1X7/MfC8QOya01JTJDZDwUpofTeN4NPIkpHV1Cpah91C1pmITeUd5XpNZK0t83P5aZXmTTBFx1ZnfE8YWxk2cnmQ3HD/PfRkGmkDkhOotxr4lYnyRSpa+pvX+KvLtR6UzB8HzHmemevT8rxsRSYbMUiexbnicz0bpSRrkFh0hcDrJeujTXYKOVHeT8cqnhTGS6ZnP02Ip0GcqzLOKJE7A/hfoLlnG8Q1eyXK3lO1gafjyewmKPbRQtpelbgPL9918JlRsT3le5LrI5RyuWwZR3C0w042llGVgSaIrYHlxuaiylyHQLFOan0fMN5NMhsNzroSKTISKQvUU+WuNITkivRNwjUej53rm0HlTUaRB6x6Ph/E8w/k0ybKW5XZJMmkV8l6LuIfnVJL9NaPkbE+8qcVH02S8gcdT6MzfrqlUxe3OrxF1TmunEV6JidKxh8CRrD9Etc1z8l6c906uWI6wGhoZ5PhpuOflnQZrOg/T0/LXKkjay/ddfBuue5JuOm5R5MjlMzpybieotuJbp8UZTNKnKpMiHTQfISKSBrYnchMKWGyzpvU/I+VOmsYbip9HzB6PIXpZ5FkDUUsL0n29LxQ8t5dHhrlJuPT8viEyMyr0OYl1nlXY+wnTdL+Q8FaUZyjMtqHJpPs/Ec3LEPXS/J9QuUmhnzyurg33XD0vwfKVTvPV69PNUw5+OrZ0xZFLS2tqkjmm6LrjPD9O45x8vD25vD0tRy7n0NgdZd+W1omtB2/ccfAuDpDa9qHJRZHhzciHJV+SOfkUZVYQuvqueRDR8wR9jpzpWVzYqsrLA8NrRppHWiTbODk66bppXN+hs8oafjLqlPK5pyDOQGlfl2Oi6T9fUrtppPt6Xi6fQdoXZ8VLp6fnT0eMppU+lvmr2TWi3Seqn0ql+Ddlui2p6qfZudcNufEvJ/TavxLo+cqCvHUNKcZNFi/Xfiq5c/Hr4pnYVcroaVObC6d0fVpsbtzXTf9d13Vd8jm1v6N0jr+WWgtd2tEmy2s/e8fCZFfae6ULHSOkJuobW1EtQ3J2XNrI5ithOhHSt2aaS0zByKXRbU7G7ZabnJgpexhdqjM4aaGb6StLaTvXFfnnrpzs2dOTOlcaS6316Xnnjouz50hKtkqqsqeh9kborUVY1T+mmiD0m1FmNNuk6HybpNpTn6Ty1i3QahGlGcuP8As8ht5L0RW5nFs76JrmBpxl07tPjmVnIjMjqVg5bFrpptz43/AEtlzZTVHRtaL25ldXQyKXIzL9718K/SfRbFOgrZXSufUT0vuIahmTspapOz7SlGdDddt5NGrhSpapLT7SpelXnG9GjZwrIUqyn5JrLpgayVvKrzrm8jKe5aZSbi/wA1eN04wjxR1ZoVeIEy2ocCtK8RO5GDTdJ9KcQvRpA7LaRqKM1StZ8TlNdJ9RTm9S1C9G0Sp9GQfK0z2h2vjRZmQ8tpSUdMM44/P1bsNRrWBk4Wh0IdsY9bprlb828P3P6fBP05bkLl0XjJqCmhTTm1hz7nTu3lx88NxT8Xri5anL9NuJ2nLcz4tK1pMU1c2T6XRDdt0XVOBg5KbFBVEvFM5HrsZTwGoo86n+YXjUtC1PvMXeeqnm9OjOviFyplNf6u8/4f2eVJSRNur/KGElo2kqfkLdF1R6LqF7os9HF7NU8XpTtLuqvOfAya5+NkdVPVMnxGwZQ19pui62Hzo3pPMP0wcak0pc9h4c7iVbyeYN5czj3Og6EO37N/PoVLWVLU9UcHlLknTh/yK7eSuLnnZ/mq8nByVCr8mPqflQvzZwuL0fsJPqtywXU5DyNMnmWcMmkrk2MqzJpkP5NnoXMMPkui9RV40NN2Gqnal29HzsWtPHNNLTSXT0fOqZV7RyeJtR6GNfGoWjS0qnQZomtE1U9bI3TM1Tv6b05psf1SaUY3HXnQ604v2NeXsqnT0jolGuaa/wBqTYDJpeU0qU0M0wcq00F0jdtNO639L5HpGbUm3NlezaTtmftY/n6BdJ60zDkHIjyac22Y7KjDn5MoayzHxTmh5PGZoxzFJGYNbKeZaxmCOUmtF1QYGlvjS6qemZPufHoeV+p2nzsGR6j0Maro49KzTMVqLvPVLdp62zJtqc2pb0hyVmSbNic012zJtGZrTSmWYmn4VzVJBYCnIeug9swRdb2OeRmcz9VryL55GZos6r//2Q==);
    background-size: auto;
    background-size:  cover;
    height: 100vh;
    transition: 0.5s;
}
.active .card{
    left: calc(100% - 500px);
}
.active .container{
   transform: translateX(-200px);
}
.card h1{
    background-image: url(data:image/jpeg;base64,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);
    background-repeat: no-repeat;
    background-size:  cover;
    font-weight: 100;
    margin: 0;
    padding: 0 20px;
    height: 80px;
    display: flex;
    align-items: center;
}
.card .checkOut{
    position: absolute;
    bottom: 0;
    width: 100%;
    display: grid;
    grid-template-columns: repeat(2, 1fr);

}
.card .checkOut div{
    background-color: #E8BC0E;
    width: 100%;
    height: 70px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: bold;
    cursor: pointer;
}
.card .checkOut div:nth-child(2){
    background-color: #1C1F25;
    color: #fff;
}
.listCard li{
    display: grid;
    grid-template-columns: 100px repeat(3, 1fr);
    color: #fff;
    row-gap: 10px;
}
.listCard li div{
    display: flex;
    justify-content: center;
    align-items: center;
}
.listCard li img{
    width: 90%;
}
.listCard li button{
    background-color: #fff5;
    border: none;
}
.listCard .count{
    margin: 0 10px;
}
#------------------------------------------------------------now java script
  let openShopping = document.querySelector('.shopping');
let closeShopping = document.querySelector('.closeShopping');
let list = document.querySelector('.list');
let listCard = document.querySelector('.listCard');
let body = document.querySelector('body');
let total = document.querySelector('.total');
let quantity = document.querySelector('.quantity');

openShopping.addEventListener('click', ()=>{
    body.classList.add('active');
})
closeShopping.addEventListener('click', ()=>{
    body.classList.remove('active');
})

let products = [
    {
        id: 1,
        name: 'กระเป๋าสตางค์ผู้ชาย',
        image: '1.PNG',
        price: 120000
    },
    {
        id: 2,
        name: 'ตุ็กตา',
        image: '2.PNG',
        price: 120000
    },
    {
        id: 3,
        name: 'ผ้าห่ม',
        image: '3.PNG',
        price: 220000
    },
    {
        id: 4,
        name: 'ตุ๊กตาหมูนิ่ม',
        image: '4.PNG',
        price: 123000
    },
    {
        id: 5,
        name: 'พวงกุญแจ',
        image: '5.PNG',
        price: 320000
    },
    {
        id: 6,
        name: 'ตุ๊กตาหมาไซบีเรียน ฮักกี้',
        image: '6.png',
        price: 120000
    }
];
let listCards  = [];
function initApp(){
    products.forEach((value, key) =>{
        let newDiv = document.createElement('div');
        newDiv.classList.add('item');
        newDiv.innerHTML = `
            <img src="image/${value.image}">
            <div class="title">${value.name}</div>
            <div class="price">${value.price.toLocaleString()}</div>
            <button onclick="addToCard(${key})">Add To Card</button>`;
        list.appendChild(newDiv);
    })
}
initApp();
function addToCard(key){
    if(listCards[key] == null){
        // copy product form list to list card
        listCards[key] = JSON.parse(JSON.stringify(products[key]));
        listCards[key].quantity = 1;
    }
    reloadCard();
}
function reloadCard(){
    listCard.innerHTML = '';
    let count = 0;
    let totalPrice = 0;
    listCards.forEach((value, key)=>{
        totalPrice = totalPrice + value.price;
        count = count + value.quantity;
        if(value != null){
            let newDiv = document.createElement('li');
            newDiv.innerHTML = `
                <div><img src="image/${value.image}"/></div>
                <div>${value.name}</div>
                <div>${value.price.toLocaleString()}</div>
                <div>
                    <button onclick="changeQuantity(${key}, ${value.quantity - 1})">-</button>
                    <div class="count">${value.quantity}</div>
                    <button onclick="changeQuantity(${key}, ${value.quantity + 1})">+</button>
                </div>`;
                listCard.appendChild(newDiv);
        }
    })
    total.innerText = totalPrice.toLocaleString();
    quantity.innerText = count;
}
function changeQuantity(key, quantity){
    if(quantity == 0){
        delete listCards[key];
    }else{
        listCards[key].quantity = quantity;
        listCards[key].price = quantity * products[key].price;
    }
    reloadCard();
}
