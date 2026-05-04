<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Hero</title>

<style>
*{margin:0;box-sizing:border-box;font-family:Arial}

.hero{
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  text-align:center;
  color:#fff;
  position:relative;
  overflow:hidden;
  background:url("https://scontent.fmnl17-6.fna.fbcdn.net/v/t39.30808-6/506512384_4113932178925978_4308809315034548879_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=dd6889&_nc_eui2=AeE2I-jVq7Mmn_QXgmigSzVVV0X1DXqviwtXRfUNeq-LC408Zy9TnHTlpuAEDCa2F3ISRmHSH0HHiqdCcodASvrB&_nc_ohc=yStgdrOaylAQ7kNvwH1w_m6&_nc_oc=AdoMMjQiCINuyj9zb93l_3XfImzXfZlt4DP8RxwYui5NIi_BkqGyh2cemS5BK4zCdyA&_nc_zt=23&_nc_ht=scontent.fmnl17-6.fna&_nc_gid=U1inY9Ct0nDunHwjto_BPw&_nc_ss=7b2a8&oh=00_Af2uqXlqoaZZ2WGf9cB7qD2rinebET17ehDKPq5mcvUlKg&oe=69F7E67A") center/cover no-repeat;
}

.hero::before{
  content:"";
  position:absolute;
  inset:0;
  background:rgba(0,0,0,.45);
}

.hero::after{
  content:"";
  position:absolute;
  width:260px;height:260px;
  border-radius:50%;
  background:rgba(255,255,255,.12);
  filter:blur(60px);
  top:-60px;left:-60px;
}

.card{
  position:relative;
  z-index:1;
  max-width:650px;
  padding:45px;
  border-radius:22px;
  background:rgba(255,255,255,.12);
  backdrop-filter:blur(18px);
  border:1px solid rgba(255,255,255,.25);
  box-shadow:0 25px 60px rgba(0,0,0,.3);
}

h1{font-size:3rem;margin-bottom:10px}
p{margin-bottom:25px;opacity:.9;line-height:1.5}

.btns{display:flex;gap:15px;justify-content:center;flex-wrap:wrap}

.btn{padding:12px 25px;border-radius:50px;text-decoration:none;font-weight:bold;transition:.3s}

.primary{background:#e60023;color:#fff}
.primary:hover{transform:translateY(-5px);box-shadow:0 15px 30px rgba(230,0,35,.4)}

.secondary{border:2px solid #fff;color:#fff}
.secondary:hover{background:#fff;color:#e60023;transform:translateY(-5px)}

@media(max-width:600px){
  h1{font-size:2.3rem}
  .card{padding:28px}
}
</style>
</head>

<body>

<section class="hero">
  <div class="card">
    <h1>Creative Web Design</h1>
    <p>
      by: Pinote, Juliana A.<br><br>
      A compilation of all activities showcasing design, creativity, and development skills.
    </p>

    <div class="btns">
      <a href="#activities" class="btn primary">Explore Work</a>
      <a href="#login" class="btn secondary">Login</a>
    </div>
  </div>
</section>

</body>
</html>
