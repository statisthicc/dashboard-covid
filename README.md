<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Best-README-Template</h3>

  <p align="center">
    An awesome README template to jumpstart your projects!
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Report Bug</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">Dashboard COVID-19</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#perancangan-desain-dashboard">Perancangan Desain Dashboard</a></li>
    <li><a href="#penjelasan-dataset">Penjelasan Dataset</a></li>
    <li><a href="#implementasi">Implementasi</a></li>
    <li><a href="#evaluasi">Evaluasi</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## Dashboard COVID-19

Severe Acute Respiratory Syndrome Coronavirus 2
(SARSCOV2) atau yang lebih dikenal dengan nama COVID-19. Virus ini dilaporkan pertama kali di kota Wuhan, Tiongkok
pada Desember 2019. COVID-19 disebabkan oleh SARS-COV2 yang termasuk dalam keluarga besar coronavirus yang
sama dengan penyebab SARS pada tahun 2003, hanya berbeda
jenis virusnya. Gejalanya mirip dengan SARS, namun angka
kematian SARS (9,6%) lebih tinggi dibanding COVID-19
(kurang dari 5%), walaupun jumlah kasus COVID-19 jauh
lebih banyak dibanding SARS. COVID-19 juga memiliki
penyebaran yang lebih luas dan cepat ke beberapa negara
dibanding SARS. COVID-19 (Coronavirus) terbukti menjadi
pandemi yang benar-benar berdampak pada orang-orang di
hampir seluruh penjuru dunia.

Kegunaan aplikasi pengolah dan visualisasi data seperti Tableau dalam analisis data COVID-19 (Coronavirus) dapat diukur dari kinerjanya, lingkungan yang ramah pengguna, dan kecepatannya. Tableau, alat yang digunakan untuk visualisasi dan penyederhanaan data kompleks, dirancang untuk membantu pengguna untuk
membuat visual dan grafik tanpa bantuan programmer atau
pengetahuan pemrograman sebelumnya. Visualisasi data
adalah cara intuitif bagi pengguna untuk dengan mudah
membaca dan memahami data, terutama dalam analisis big data. Selain itu, visualisasi data juga membantu untuk
meningkatkan kualitas tata kelola kebijakan atau layanan
dengan menghadirkan pandangan dan bukti yang terintegrasi
dan dapat dipertanggungjawabkan untuk membuat suatu
keputusan.

Salah satu bentuk visualisasi data yaitu dashboard.
Dashboard merupakan visualisasi dari informasi penting yang
diperlukan untuk mencapai suatu tujuan, ditampilkan dalam
sebuah layar, informasi yang ditampilkan dapat dengan mudah
dianalisis. Informasi yang ditampilkan pada dashboard dalam
bentuk grafik yang berfungsi untuk memudahkan manusia
dalam memahami informasi. Oleh karena itu, berdarkan latar belakang dan masalah diatas, tujuan dari penelitian ini yaitu membuat dashboard interaktif dengan menggunakan Tableau

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

Dashboard ini dibuat menggunakan Tableu Public untuk desain dashboard dan R untuk preprocessing data.

- [Tableau Public](https://public.tableau.com/en-us/s/)
- [R](https://cran.r-project.org/bin/windows/base/)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- GETTING STARTED -->

## Perancangan Desain Dashboard

Perancangan dashboard seperti yang didapat pada hasil studi
literatur bahwa untuk membuat suatu dashboard yang ideal
perlu memperhatikan dua aspek utama, yaitu memilih data
yang tepat dan memilih teknik visualisasi yang tepat. Untuk
dapat memilih data yang tepat dapat menggunakan model
GQM (Goal-Question-Measurement).
Sebuah model GQM didefinisikan menjadi tiga level, yaitu: 1. _The goal_, 2. _The questions_, dan 3. _The measures_

![GQM Model](/images/gqm.png)

Sedangkan agar dapat memilih teknik visualisasi yang tepat
dapat digunakan pendekatan dua skenario penggunaan
dashboard, yaitu “pull” dan “push”.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->

## Penjelasan Dataset

Data diambil dari dataset publik pada situs Kaggle (https://www.kaggle.com/datasets/hendratno/covid19-indonesia) yang berisi tentang data harian COVID-19 di
Indonesia mulai tanggal 1 Maret 2020 – 3 Desember 2021 yang
dirangkum dari beberapa situs resmi, seperti: covid19.go.id,
kemendagri.go.id, bps.go.id, dan bnpb.inacovid19.hub.arcgis.com

Dataset terdiri 38 kolom dan 21759 observasi.

![Summary Dataset](/images/summary.png)

Dari dataset tersebut data yang digunakan yaitu Date, Location ISO Code, Location, New Cases, New Deaths, New Recovered, New Active Cases,Total Cases, Total Deaths, Total Recovered dan Total Active Cases. Karena pada data Date dan data kuantitatif (New Cases,...,Total active cases) yang digunakan tersebut tidak terdapat Missing Value, sehingga tidak perlu untuk melakukan preprocessing data.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ROADMAP -->

## Implementasi

Adapun tahapan implementasi desain dashboard yang sudah dibuat sebagai berikut

1. Membuat Peta Sebaran COVID-19
2. Membuat visualisasi teks
3. Membuat visualisasi berupa line chart dan bar chart
4. Membuat dashboard dari visualisasi 1-3

Berikut ini merupakan hasil akhir dashboard COVID-19 menggunakan Tableau

![Tampilan Dashboard](/images/dashboard.png)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTING -->

## Evaluasi

Untuk evaluasi visualisasi dapat menggunakan berbagai metode, beberapa contohnya yaitu survei dengan System Usability Scale yang sudah dimodifikasi untuk visualisasi data dan Focus Group Methodology (FGD). Namun, karena keterbatasan waktu pada penelitian kali ini belum dilakukan evaluasi hasil visualisasi dashboard.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- LICENSE -->

## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->

## Contact

Muhamad Ridwan - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
