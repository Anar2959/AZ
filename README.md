<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta http-equiv="X-UA-compaible" content="ie=edge" />
    <link rel="stylesheet" type="text/css" href="./style.css" />
    <title> AZ online library </title>

    <style>
        body {
            background-image: url("header_pic1.jpg");
            font-family: courier;
            
        }
        #page-wrap {
            width: 1000px;
            margin: 0 auto;
        }

        h1 {
            text-align: center;
            color: #00e6e6;
            font-size: 50px;
        }

        h2 {
            text-align: center;
            color: #00e6e6;
            font-size: 20px;
        }

        .menuitem {
            margin-top: 50px;
            margin-left: 10px;
            display: inline-block;
            padding: 10px;
            border: 1px solid rgb(204, 255, 255);
            border-radius: 1px;
            background-color: darkslategrey;
            width: 150px;
            height: 20px;
        }

        a {
            color: white;
            text-decoration: none;
            text-align: center;
            display: block;
        }


        .search {
            width: 100%;
            position: relative;
            display: flex;
        }

        .searchTerm {
            width: 100%;
            border: 3px solid #00e6e6;
            border-right: none;
            padding: 5px;
            height: 20px;
            border-radius: 5px 0 0 5px;
            outline: none;
            color: #9DBFAF;
        }

            .searchTerm:focus {
                color: #00e6e6;
            }

        .searchButton {
            width: 40px;
            height: 36px;
            border: 1px solid #00e6e6;
            background: #00e6e6;
            text-align: center;
            color: #fff;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
            font-size: 20px;
        }

        /*Resize the wrap to see the search bar change!*/
        .wrap {
            width: 700px;
            position: absolute;
            top: 500px;
            left: 50%;
            transform: translate(-50%, -50%);
        }

        .new_things {
            margin-top: 200px;
            color: #ffcc00;
            font-size: 20px;
            float: left;
        }

            .new_things img {
                width: 150px;
                height: 200px;
            }

            .new_things li {
                display: inline-block;
                text-decoration: none;
                margin-top: 50px;
            }

        .reading {
            margin: 0;
            padding: 0;
        }

            .reading img {
                display: inline-block;
                margin-left: 50px;
            }

            .reading a {
                font-size: 12px;
            }

            .reading hr {
                width: 150px;
            }

        .about a:hover {
            color: red;
        }

        /* Next & previous buttons 
        .prev, .next {
            cursor: pointer;
            position: absolute;
            top: 120%;
            width: auto;
            margin-top: -30px;
            padding: 16px;
            color: #00e6e6;
            font-weight: bold;
            font-size: 20px;
            border-radius: 0 3px 3px 0;
            user-select: none;
        }

        .next {
            position: absolute;
            right: 300px;
            border-radius: 3px 0 0 3px;
        }

            .prev:hover, .next:hover {
                background-color: rgba(0,0,0,0.8);
                color: #ffcc00;
            }

        .slideshow-container {
            position: relative;
        }
            */

        .mySlide {
            text-align: center;
        }

        .best_things {
            margin-top: 700px;
            color: #ffcc00;
            font-size: 20px;
        }

            .best_things_aguulga, .card {
                display: inline-block; 
                margin-left: 25px; 
            }

            .card {
                box-shadow: 4px 4px 8px 8px rgba(0,0,0,0.2);
                transition: 0.7s;
                width: 30%;
                font-size: 12px;
                border-radius: 5px;
            }

                .card:hover {
                    box-shadow: 0 8px 16px 0 rgba(0,230,230, 0.8);
                    border-radius: 5px;
                }

                .container {
                    padding: 2px 16px;
                    background-color: rgb(255, 255, 255, 0.2);
                }

                .card img {
                    width: 200px;
                    height: 300px;
                    border-radius: 5px;
                }

        .free_things {
            margin-top: 100px;
            color: #ffcc00;
            font-size: 20px;
            float: left;
        }

            .free_things img {
                width: 150px;
                height: 200px;
            }

            .free_things li {
                display: inline-block;
                text-decoration: none;
                margin-top: 50px;
            }

        .english_things {
            margin-top: 100px;
            color: #ffcc00;
            font-size: 20px;
            float: right;
           
        }

            .english_things hr{
                width: 1000px; 
            }

            .english_things_aguulga, .card1 {
                display: inline-block;
                margin-left: 22px;
            }

        .card1 {
            box-shadow: 4px 4px 8px 8px rgba(0,0,0,0.2);
            transition: 0.7s;
            width: 30%;
            font-size: 12px;
            border-radius: 5px;
            background-color: rgb(0, 0, 0, 0.6);
        }

            .card1:hover {
                box-shadow: 0 8px 16px 0 rgba(0,230,230, 0.8);
                border-radius: 5px;
            }

        .container {
            padding: 2px 16px;
            background-color: rgb(255, 255, 255, 0.2);
        }

        .card1 img {
            width: 200px;
            height: 300px;
            border-radius: 5px;
        }

        footer {
            margin-top: 1200px;
            color: #ffcc00;
            font-size: 20px;
        }

        footer p {
            color: #00e6e6;
            font-size: 20px;
        }

            .about, .card2 {
                display: inline-block;
                margin-left: 22px;
            }

            .card2 {
                box-shadow: 4px 4px 8px 8px rgba(0,0,0,0.2);
                transition: 0.7s;
                width: 30%;
                font-size: 12px;
                border-radius: 5px;
                background-color: rgb(204, 255, 255, 0.2);
            }

                .card2:hover {
                    box-shadow: 0 8px 16px 0 rgba(0,230,230, 0.8);
                    border-radius: 5px;
                }

                .container {
                    padding: 2px 16px;
                    background-color: rgb(255, 255, 255, 0.2);
                }

                .card2 img {
                    width: 70px;
                    height: 200px;
                    border-radius: 5px;
                }
         
    </style>

</head>

<body id="page-wrap">
    <section>
          
        <heading>
            <nav class="title">
                <h1> ЦАХИМ НОМЫН САН <img src="az_logo.png" width="200px" height="140px"> </h1>
                <h2 style="color: #ffcc00"><i>"БИД ГАНЦААРАА БИШ ГЭДГЭЭ МЭДЭХИЙН ТУЛД НОМ УНШДАГ"</i></h2>
            </nav>

            <nav class="nav">
                <ul>
                    <li class="menuitem"><a href="">НҮҮР</a></li>
                    <li class="menuitem"><a href="">УНШДАГ НОМ</a></li>
                    <li class="menuitem"><a href="">СОНСДОГ НОМ</a></li>
                    <li class="menuitem"><a href="">СЭТГҮҮЛ</a></li>
                    <li class="menuitem"><a href="">САНАЛ ХҮСЭЛТ</a></li>
                </ul>
            </nav>
        </heading>
        <nav class="wrap">
            <nav class="search">
                <input type="text" class="searchTerm" placeholder="Номын гарчгийг оруулна уу">
                <button type="submit" class="searchButton">
                    <i class="fa fa-search"></i>
                </button>
            </nav>
        </nav>
    </section>
    <section1>
        <nav class="new_things">
            <p><b>ШИНЭЭР НЭМЭГДСЭН</b><hr></p>
            <div class="mySlide">
                <ul>

                    <li class="reading">
                        <img src="nom_1.jpg">
                        <hr />

                        <a href="">
                            Дээврийн өрөөн дэхь <br /> миний мөрөөдөл 
                        </a>
                    
                    </li>
                    <li class="reading">
                        <img src="nom_2.jpg">
                        <hr />
                        <a href="">
                            Бидний харж чадахгүй
                            <br />гэрэл гэгээ
                        </a>
                    </li>
                    <li class="reading">
                        <img src="nom_3.jpg">
                        <hr />
                        <a href="">Алхимич <br />-Адал явдалт түүх</a>
                    </li>
                    <li class="reading">
                        <img src="nom_4.jpg">
                        <hr />
                        <a href="">Ад үзэгдэх зориг <br /> -Адлерийн сэтгэл судлал </a>
                    </li>
                </ul>
            </div>

           <!--<a class="prev" onclick="plusSlides(-1)">❮</a>
            <a class="next" onclick="plusSlides(1)">❯</a>--> 

         
            <!--<script>
                var slideIndex = 1;
                showSlides(slideIndex);

                function plusSlides(n) {
                    showSlides(slideIndex += n);
                }

                function currentSlide(n) {
                    showSlides(slideIndex = n);
                }

                function showSlides(n) {
                    var i;
                    var slides = document.getElementsByClassName("mySlides");
                    var dots = document.getElementsByClassName("dot");
                    if (n > slides.length) { slideIndex = 1 }
                    if (n < 1) { slideIndex = slides.length }
                    for (i = 0; i < slides.length; i++) {
                        slides[i].style.display = "none";
                    }
                    for (i = 0; i < dots.length; i++) {
                        dots[i].className = dots[i].className.replace(" active", "");
                    }
                    slides[slideIndex - 1].style.display = "block";
                    dots[slideIndex - 1].className += " active";
            </script>-->

        </nav>
    </section1>
    <section2>
        <nav class="best_things">
            <p><b>ЭНЭ САРЫН ОНЦЛОХ НОМООР</b><hr /></p>
            <nav class="best_thing_aguulga">
                <div class="card">
                    <img src="philo_1.jpg" alt="best_book" style="width:100%;">
                    <div class="container">
                        <h4 style="font-size: 20px; color: #00e6e6"><b>Философи, математик бас бус</b></h4>
                        <p style="color: white">
                            Эрхлэн гаргасан: Garuna publishing
                            <br />
                            ISBN: 978-99199-5-722-3
                            <br />
                            Хавтас: Зөөлөн
                            <br />
                            Хэвлэгдсэн он: 2020
                            <br />
                            Хуудас: 220
                            <br />
                            Хэмжээ: 181*129мм
                            <br />
                            Жин: 221
                            <br />
                        </p>
                    </div>
                </div>
                <div class="card">
                    <img src="philo_1.jpg" alt="best_book" style="width:100%">
                    <div class="container">
                        <h4 style="font-size: 20px; color: #00e6e6"><b>Философи, математик бас бус</b></h4>
                        <p style="color: white">
                            Эрхлэн гаргасан: Garuna publishing
                            <br />
                            ISBN: 978-99199-5-722-3
                            <br />
                            Хавтас: Зөөлөн
                            <br />
                            Хэвлэгдсэн он: 2020
                            <br />
                            Хуудас: 220
                            <br />
                            Хэмжээ: 181*129мм
                            <br />
                            Жин: 221
                            <br />
                        </p>
                    </div>
                </div>
                <div class="card">
                    <img src="philo_1.jpg" alt="best_book" style="width:100%">
                    <div class="container">
                        <h4 style="font-size: 20px; color: #00e6e6"><b>Философи, математик бас бус</b></h4>
                        <p style="color: white">
                            Эрхлэн гаргасан: Garuna publishing
                            <br />
                            ISBN: 978-99199-5-722-3
                            <br />
                            Хавтас: Зөөлөн
                            <br />
                            Хэвлэгдсэн он: 2020
                            <br />
                            Хуудас: 220
                            <br />
                            Хэмжээ: 181*129мм
                            <br />
                            Жин: 221
                            <br />
                        </p>
                    </div>
                </div>
            </nav>
        </nav>
    </section2>
    <section3>
        <nav class="free_things">
            <p><b>САНАЛ БОЛГОХ ҮНЭГҮЙ НОМНУУД</b><hr /></p>
                  <div class="mySlide">
                <ul>

                    <li class="reading">
                        <img src="nom_1.jpg">
                        <hr />

                        <a href="">
                            Дээврийн өрөөн дэхь <br /> миний мөрөөдөл 
                        </a>
                    
                    </li>
                    <li class="reading">
                        <img src="nom_2.jpg">
                        <hr />
                        <a href="">
                            Бидний харж чадахгүй
                            <br />гэрэл гэгээ
                        </a>
                    </li>
                    <li class="reading">
                        <img src="nom_3.jpg">
                        <hr />
                        <a href="">Алхимич <br />-Адал явдалт түүх</a>
                    </li>
                    <li class="reading">
                        <img src="nom_4.jpg">
                        <hr />
                        <a href="">Ад үзэгдэх зориг <br /> -Адлерийн сэтгэл судлал </a>
                    </li>
                </ul>
            </div>

            <!--<a class="prev" onclick="plusSlides(-1)">❮</a>
            <a class="next" onclick="plusSlides(1)">❯</a>

         
            <script>
                var slideIndex = 1;
                showSlides(slideIndex);

                function plusSlides(n) {
                    showSlides(slideIndex += n);
                }

                function currentSlide(n) {
                    showSlides(slideIndex = n);
                }

                function showSlides(n) {
                    var i;
                    var slides = document.getElementsByClassName("mySlides");
                    var dots = document.getElementsByClassName("dot");
                    if (n > slides.length) { slideIndex = 1 }
                    if (n < 1) { slideIndex = slides.length }
                    for (i = 0; i < slides.length; i++) {
                        slides[i].style.display = "none";
                    }
                    for (i = 0; i < dots.length; i++) {
                        dots[i].className = dots[i].className.replace(" active", "");
                    }
                    slides[slideIndex - 1].style.display = "block";
                    dots[slideIndex - 1].className += " active";
            </script>-->

        </nav>
    </section3>
    <section4>
        <nav class="english_things">
            <p>
                <b>ТАНЫ ГАДААД ХЭЛНИЙ МЭДЛЭГТ</b>
                <hr />
            </p>

            <nav class="english_things_aguulga">
                <div class="card1">
                    <img src="harry_1c.png" alt="best_book" style="width:100%;">
                    <div class="container">
                        <h4 style="font-size: 20px; color: #00e6e6"><b>Harry Potter and the Half Blood Prince</b></h4>
                        <p style="color: white">
                            <a href="">ЦААШ ҮЗЭХ</a>
                            <br />
                         
                        </p>
                    </div>
                </div>
                <div class="card1">
                    <img src="harry_2c.png" alt="best_book" style="width:100%">
                    <div class="container">
                        <h4 style="font-size: 20px; color: #00e6e6"><b>Harry Potter and the Chamber of Secrets</b></h4>
                        <p style="color: white">
                            <a href="">ЦААШ ҮЗЭХ</a>
                            <br />

                        </p>
                    </div>
                </div>
                <div class="card1">
                    <img src="harry_3c.png" alt="best_book" style="width:100%">
                    <div class="container">
                        <h4 style="font-size: 20px; color: #00e6e6"><b>Harry Potter and the Goblet of Fire</b></h4>
                        <p style="color: white">
                            <a href="">ЦААШ ҮЗЭХ</a>
                            <br />

                        </p>
                    </div>
                </div>
            </nav>
        </nav>
    </section4>
    <footer>
        <nav class="about">
            <p>
                <b>БИДНИЙ ТУХАЙ</b>
                <hr />
            </p>
            <p>
                Нийт гишүүний тоо: 3
                <br />
                Номын сангийн эх сурвалж: 
                <br />
                /Дээр нь дараад тухайн хуудас руу зочлох боломжтой/
                <br />
                <a href="http://mn-nom.blogspot.com/" style="color: whitesmoke">Betterman's Blog</a>
                <br />
                <a href="https://book.mn/">Аз Хур Номын Худалдааны Хуудас</a>
                <br />
                <a href="https://www.mplus.mn/">M Plus Цахим Номын Худалдааны Хуудас </a>
                <br />
                <a href="https://www.scribd.com/">Scribd.com</a>
                <br />
                Үүсгэн байгуулагдсан он: 2020.10

            </p>
            <div class="card2">
                <img src="avatar.png" alt="about_1" style="width:100%;">
                <div class="container">
                    <h4 style="font-size: 20px; color: #00e6e6"><b>Батболдын Анар</b></h4>
                    <p style="color: white">
                        Хичээл: Веб програмчлал
                        <br />
                        ID: 18B1NUM2959
                        <br />
                        Түвшин: 3
                        <br />
                        Холбоо барих цахим хаяг: 18B1NUM2959@
                        <br />
                        stud.num.edu.mn
                    </p>
                </div>
            </div>
            <div class="card2">
                <img src="avatar_1.png" alt="about_1" style="width:100%;">
                <div class="container">
                    <h4 style="font-size: 20px; color: #00e6e6"><b>Батсүхийн Зуунбилэг</b></h4>
                    <p style="color: white">
                        Хичээл: Веб програмчлал
                        <br />
                        ID: 18B1NUM1220
                        <br />
                        Түвшин: 3
                        <br />
                        Холбоо барих цахим хаяг: 18B1NUM1220@
                        <br />
                        stud.num.edu.mn
                    </p>
                </div>
            </div>
            <div class="card2">
                <img src="avatar_2.png" alt="about_1" style="width:100%;">
                <div class="container">
                    <h4 style="font-size: 20px; color: #00e6e6"><b>Батсүрэнгийн Батбилэг</b></h4>
                    <p style="color: white">
                        Хичээл: Веб програмчлал
                        <br />
                        ID: 17B1NUM0257
                        <br />
                        Түвшин: 4
                        <br />
                        Холбоо барих цахим хаяг: 17B1NUM0257@
                        <br />
                        stud.num.edu.mn
                    </p>
                </div>
            </div>
            </nav>
</footer>

</body>
</html>



