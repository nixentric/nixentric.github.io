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

Sampai disini mungkin diantara kita ada yang **bertanya**: Lantas, apa yang membedakan Tailwind CSS dengan framework yang lain, bukankah framework lain juga menawarkan kemudahan dalam mendesain sebuah website juga?

Untuk membahas itu, mari kita menuntaskan terlebih dahulu definisi dari Tailwind CSS, serta kelebihan dan kekurangan menggunakan framework ini. Sehingga kamu dapat menentukan, apakah framework ini tepat untukmu atau malah sebaliknya.

## Definisi Tailwind CSS
Seperti yang kita singgung sebelumnya, Tailwind CSS merupakan framework yang berbasis Utility-First. Lantas, apa yang dimaksud dengan Utility-First CSS? Utility-First CSS merupakan sebuah konsep framework CSS yang berbasis low-level class, yang artinya setiap class hanya memiliki 1 fungsi.

### Contoh:
Apabila kita ingin membuat

<div class="chat-notification">
  <div class="chat-notification-logo-wrapper">
    <img class="chat-notification-logo" src="/img/logo.svg" alt="ChitChat Logo">
  </div>
  <div class="chat-notification-content">
    <h4 class="chat-notification-title">ChitChat</h4>
    <p class="chat-notification-message">You have a new message!</p>
  </div>
</div>

<style>
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
</style>

Hal inilah yang membedakan Tailwind CSS dengan kebanyakan framework CSS populer lainnya seperti Bootstrap, Foundation dan lain sebagainya.

First-Utility framework sebenarnya juga bukan hal yang baru di dunia framework CSS itu sendiri, ada beberapa diantaranya bla,bla. Bahkan diantaranya telah lahir sebelum tailwind CSS ini muncul. Namun kenapa tailwind CSS yang populer?
