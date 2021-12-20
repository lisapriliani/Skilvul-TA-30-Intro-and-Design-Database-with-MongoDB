<h1> Nomor 1 </h1>
<p> Skema DB profile pengguna aplikasi Skiljek</p>
<ul>
<li>Full Name</li>
<li>Email</li>
<li>Phone Number</li>
</ul>

<b>Relationships : One-to-One</b>

```js
{
"_id":{"$oid":"61c0dae2b9bbfc254c814ff9"},
"fullName":"Lisa Apriliani",
"email":"lisapriliani@gmail.com",
"phoneNumber":"0897836490"
}
```

<h1> Nomor 2 </h1>
<p> Skema DB data alamat pengguna SkilShop</p>
<ul>
<li>Full Name</li>
<li>Phone Number</li>
<li>Address (max 2)</li>
</ul>

<b>Relationships : One-to-Few</b>

```js
{
    "_id":{"$oid":"61c0e012b9bbfc254c814ffc"},
    "fullName":"Lisa Apriliani",
    "phoneNumber":"09873674939",
    "address":[
        {
            "street":"Jl.cempaka 123",
            "type":"kost"
        },
        {
            "street":"jalan kaliurang",
            "type":"rumah"
            }
        ]}
```

<h1> Nomor 3 </h1>
<p> Skema DB data dari Productsdari aplikasi SkilShop </p>
<ul>
<li>Product Name</li>
<li>Variant</li>
<li>Brand Name</li>
</ul>

<b>Relationships : One-to-Many</b>

```js
{
    "_id":{"$oid":"61c0e426b9bbfc254c814fff"},
    "productName":"Kaos Polos",
    "brandName":"SkilShirt",
    "variants":[
            {
                "variant_name":"Kaos Polos Hitam",
                "color":"Hitam",
                "quantity":"12",
                "price":"Rp. 99000"
            },
            {
                "variant_name":"Kaos Polos Navy",
                "color":"Navy",
                "quantity":"10",
                "price":"Rp. 99000"
                }
            ]
}

```
