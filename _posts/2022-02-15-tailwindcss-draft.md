---
layout: post
title:
date: 2024-02-13 11:11:11 +07:00
description: Selamat datang teman-teman
tag:
  - CSS
  - Tailwind CSS
permalink: /:categories/:title
---
Tailwind CSS, merupakan framework yang belakangan sedang naik daun di kalangan pengembang website di tahun 2022 ini. Pasalnya, framework ini menawarkan sebuah konsep menarik yang dinamakan utility-first CSS framework, dimana dengan menggunakan framework ini proses styling akan menjadi lebih cepat, serta kebebasan dan kemudahan dalam mendesain sebuah website.

Lantas, apa yang membedakan Tailwind CSS dengan framework yang lain, bukankah framework lain juga menawarkan kemudahan dalam mendesain sebuah website juga?

Untuk membahas itu, mari kita menuntaskan terlebih dahulu definisi dari Tailwind CSS, serta kelebihan dan kekurangan menggunakan framework ini. Sehingga kamu dapat menentukan, apakah framework ini tepat untukmu atau malah sebaliknya.

## Definisi Tailwind CSS
Seperti yang kita singgung sebelumnya, Tailwind CSS merupakan framework yang berbasis Utility-First. Maksud dari Utility-First adalah sebuah konsep framework CSS berbasis low-level class, yang artinya setiap class hanya memiliki 1 fungsi.

### Contoh:
Kita ingin membuat sebuah card seperti gambar dibawah ini:

<p align="center">
<img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhwyVx0LRBS8fkxthnr8RrmwBPYavVy35knbtM4k3_5iDulnfXgQv6aYspnHxTTlH_9FmmkJosDO6EH52kPIZSqhM75P9r-dVu8-1hpgMIFWDoW_GOwUmbLZ17GVUk2CoZUoRNqUG2fYBeeb9_6FmJgi_nmZFfYXaBrMuzdYJjaZ9t6EcCsfTlypTaiAA/s384/contoh-card.png" alt="Contoh Card yang dibuat dengan TailwindCSS"></p>

Jika pendekatan dengan metode tradisional, kita biasanya akan membuat satu class khusus hanya untuk satu desain saja, contohnya sebagai berikut:

#### Kode HTML dengan Pendekatan Tradisional 
```html
<div class="chat-notification">
  <div class="chat-notification-logo-wrapper">
    <img class="chat-notification-logo" src="/img/logo.svg" alt="ChitChat Logo">
  </div>
  <div class="chat-notification-content">
    <h4 class="chat-notification-title">ChitChat</h4>
    <p class="chat-notification-message">You have a new message!</p>
  </div>
</div>
```
#### Kode CSS dengan Pendekatan Tradisional
```css
  .chat-notification {
    display: flex;
    max-width: 24rem;
    margin: 0 auto;
    padding: 1.5rem;
    border-radius: 0.5rem;
    background-color: #fff;
    box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
  }
  .chat-notification-logo-wrapper {
    flex-shrink: 0;
  }
  .chat-notification-logo {
    height: 3rem;
    width: 3rem;
  }
  .chat-notification-content {
    margin-left: 1.5rem;
    padding-top: 0.25rem;
  }
  .chat-notification-title {
    color: #1a202c;
    font-size: 1.25rem;
    line-height: 1.25;
  }
  .chat-notification-message {
    color: #718096;
    font-size: 1rem;
    line-height: 1.5;
  }
```

Sedangkan, jika kita menggunakan framework Tailwind CSS, kita hanya perlu mengombinasikan beberapa class di dalam tag element tanpa perlu menulis CSS, sehingga membuat pekerjaan kita lebih cepat dan effisien.

```html
<div class="p-6 max-w-sm mx-auto bg-white rounded-xl shadow-lg flex items-center space-x-4">
  <div class="shrink-0">
    <img class="h-12 w-12" src="/img/logo.svg" alt="ChitChat Logo">
  </div>
  <div>
    <div class="text-xl font-medium text-black">ChitChat</div>
    <p class="text-slate-500">You have a new message!</p>
  </div>
</div>
```

## Perbedaan Tailwind CSS dengan Framework Populer Lainnya

Dari contoh di atas, jika kita pernah menggunakan framework populer lain, seperti Bootstrap, Bulma dan lain sebagainya, kita dapat melihat perbedaan Tailwind CSS dengan kebanyakan framework populer lainnya.

Mulai dari konsep, Tailwind menggunakan pendekatan Utility-First, sedangkan kebanyakan framework populer lain mengadaptasi konsep UI Kit. Yang mana UI Kit memiliki komponen template dan siap pakai. Contohnya saja, jika kita ingin membuat button, maka Bootstrap hanya melakukan hal berikut ini:

```html
<button type="button" class="btn btn-primary">Primary</button>
```

Sedangkan Tailwind:
```html
<button type="button" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">Primary</button>
```

Kalau dilihat dari kedua kode tersebut, Bootstrap tampak lebih simpel dan lebih efisien. Namun, karena konsep bootstrap adalah UI Kit, ia meninggalkan sebuah tanda atau style bahwa kita menggunakan

Kekurangan:
- Karena

First-Utility framework sebenarnya juga bukan hal yang baru di dunia framework CSS itu sendiri. Ada beberapa diantaranya tachyons, basscss, shed-css, dan masih banyak lagi. Bahkan diantaranya telah lahir sebelum tailwind CSS ini muncul. Namun kenapa tailwind CSS yang populer?
