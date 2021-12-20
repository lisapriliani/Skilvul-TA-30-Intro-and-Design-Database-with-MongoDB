<h1> Nomor 1 </h1>
<p> Skema DB profile pengguna aplikasi Skiljek</p>
<ul>
<li>Full Name</li>
<li>Email</li>
<li>Phone Number</li>
</ul>

<b>Relationships : One-to-One</b>

```
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
```
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

