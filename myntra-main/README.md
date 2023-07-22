<h1 align="center" style="color:blue"><b>The Myntra Clone</b></h1>

<br>

<p align="center">
<img style="display:block; margin:auto; " src="https://myntradine.netlify.app/images/mainLogo.png" width="230px" alt="Error 404">
</p>

<br>

## Project Name : `MYNTRA`

<br>

# About :

<b>Myntra ia an E-commerce site where user can login or signup and buy diffrent things like myntra.com. User also can sort and filter the products.</b>

<br>

## Deployed Link :

   - Frontend: <a href="https://myntradine.netlify.app/">Netlify</a>
   - Backend: <a href="https://myntra-tun3.onrender.com">Render</a>


<br>

# Requirements : 

- User can log in and sign up
    -Used Bcrypt and Jsonwebtoken
- User can visit pages 
- Users can see products 
- User can add products to wishlist
    - User can view wishlist 
    - User adds products from wishlist to cart
    - User can cancel a product
    - User can place an order
    - User can pay the amount
- Logout 

<br>



<br>

# Tech stack :

### Frontend 

- HTML
- CSS
- JavaScript

### Backend 

- Node.js 
- Express.js

### Database

- MongoDB 


# Schema : 

- User 
      - name: { type: String, required: true, maxLength: 15, minLength: 4 },
     - email: {
      type: String,
      required: true,
      unique: true,
      validate validator.isEmail,
    },
    - pass: {
      type: String,
      required: true,
      minLength: 4,
    },
    - phone: {
      type: String,
      required: true,
      minLength: 10,
    }


- Products 
    - image_url: { type: Object, required: true },
   - brand: { type: String, required: true },
    - subtext: { type: String, required: true },
   - price: { type: Number, required: true },
   - mrp: { type: Number, required: true },
    -offer: { type: Number, required: true },
   - category: { type: String, required: true },
   - gender: { type: String },
   - rating:{type:Number},
   - discount:{type:Number}

- cart 
   -  userID: { type: String, required: true },
 - title: { type: String, required: true },
 - image: { type: String, required: true },
 - price: { type: Number, required: true },
 - desc: { type: String, required: true },
 - qty: { type: Number, required: true },

<br>


## Run Locally

Clone the project

```bash
  git clone https://github.com/aniketbabariya24/myntra.git
```

Go to the project directory

```bash
  cd Backend
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```
------------
<br>

<h2>HomePage</h2>
<img src="https://github.com/aniketbabariya24/myntra/assets/112626195/1ff84aae-c04f-4230-a995-b82812121447" alt="">

<br>

<h2>Sign In / Sign Up page</h2>
<img src="https://github.com/aniketbabariya24/myntra/assets/112626195/9e0692f5-0d72-4668-95f1-98cc3f431540" alt="">


<br>

<h2>Product Page</h2>
<img src="https://github.com/aniketbabariya24/myntra/assets/112626195/62e60589-3b06-4839-ba45-8e1fa4ccae1d" alt="">


<br>

<h2>Wishlist Page</h2>
<img src="https://github.com/aniketbabariya24/myntra/assets/112626195/c6b76f31-6426-4562-b00e-41188a6b7802" alt="">

<br>

<h2>Cart Page</h2>
<img src="https://github.com/aniketbabariya24/myntra/assets/112626195/ccb99bb1-3d42-45e8-a21a-cc77c3bbf5a7" alt="">

<br>
