# Tutorial 4 Game Development

## Tutorial

### 1. Pembuatan TileMap dan TileSet

Saya memulai dengan menambahkan node `TileMapLayer` ke dalam scene Level1. Kemudian saya membuat TileSet baru dan mengatur ukuran tile menjadi 128x128 sesuai dengan ukuran spritesheet yang digunakan.

### 2. Penambahan Collision pada Tile

Agar player dapat berinteraksi dengan lingkungan, saya menambahkan Physics Layer pada TileSet. Kemudian saya menggambar collision shape untuk setiap tile yang digunakan.

### 3. Implementasi Kamera

Saya menambahkan node `Camera2D` sebagai child dari player agar kamera dapat mengikuti pergerakan player secara otomatis.

### 4. Implementasi Win dan Lose Condition dengan Signal

Saya membuat sebuah scene berbasis `Area2D` yang berfungsi sebagai trigger untuk kondisi menang dan kalah.

Dengan menggunakan signal `body_entered`, saya menghubungkan event ketika player masuk ke area tertentu. Jika player mencapai area goal, maka scene akan berpindah ke layar kemenangan. Jika player jatuh ke jurang, maka level akan diulang.

### 5. Implementasi Obstacle (Ikan Jatuh)

Saya membuat sebuah scene baru untuk obstacle berupa ikan dengan root node `RigidBody2D`. Di dalamnya terdapat `Sprite2D` dan `CollisionShape2D`.

Saya menambahkan script agar ketika player bertabrakan dengan objek ikan, maka permainan akan berakhir atau player kalah.


### 6. Implementasi Spawner

Saya membuat sistem spawner menggunakan node `Node2D` yang akan menghasilkan obstacle secara berkala.

## Latihan Mandiri

### 1. Level Baru dengan TileMap Berbeda

Saya menggunakan TileMap yang berbeda dari level pertama untuk menciptakan variasi visual dan desain level yang baru.


### 2. Obstacle Berbeda

Selain obstacle ikan pada level pertama, saya menambahkan jenis obstacle lain pada level baru untuk memberikan variasi tantangan kepada pemain.

### 3. Kombinasi Rintangan

Level baru memiliki:

* Jurang sebagai rintangan statis
* Obstacle yang jatuh secara periodik menggunakan spawner

## Polishing

Untuk meningkatkan kualitas permainan, saya menambahkan beberapa elemen tambahan:

### 1. Background Berbeda untuk Setiap Level

Setiap level memiliki background yang berbeda sehingga memberikan variasi visual dan suasana yang lebih menarik.

### 2. Background Music

Saya menambahkan background music pada setiap level agar pengalaman bermain menjadi lebih hidup dan tidak terasa kosong.

Assets used:

- Background images: https://free-game-assets.itch.io/nature-landscapes-free-pixel-art?download
- Background music: https://www.youtube.com/watch?v=hrgzWEgCCFg&list=PLwJjxqYuirCLkq42mGw4XKGQlpZSfxsYd&index=2
