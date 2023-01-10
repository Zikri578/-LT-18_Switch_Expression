# -LT-18_Switch_Expression

Switch expressions di JavaScript adalah fitur baru yang ditambahkan ke versi ECMAScript 2020 (ES11) yang meningkatkan kemampuan switch statement. Seperti switch statement biasa, switch expression mengevaluasi suatu ekspresi dan mengeksekusi blok kode yang sesuai dengan nilai ekspresi tersebut. Namun, dengan switch expression, kamu dapat menggunakan sintaks yang lebih ringkas dan elegan. Berikut adalah contoh sederhana dari switch expression:

    const value = "A";
    const result = switch (value) {
      case "A":
        yield "Value is A";
      case "B":
        yield "Value is B";
      default:
        yield "Value is something else";
    }
    console.log(result.next().value);

Dalam contoh di atas, variable value diinisialisasi dengan nilai "A". Kemudian, switch expression mengevaluasi variable `value` dan mengeksekusi case yang sesuai. Karena nilai `value` adalah "A", case "A" dijalankan dan menghasilkan "Value is A".

Perbedaan lainnya dari switch expression adalah dapat mengeluarkan return langsung dari case, tidak perlu menggunakan break atau return, dan dapat menggunakan yield statement pada setiap case.

Selain itu, switch expression juga memiliki sintaks yang lebih fleksibel daripada switch statement biasa. Kamu dapat menggunakan operator `arrow function `(=>)` untuk menuliskan kode yang lebih ringkas dan elegan. Berikut ini adalah contoh:

    const value = "A";
    const result = switch (value) {
      case "A":
        yield "Value is A";
      case "B":
        yield "Value is B";
      default:
        yield "Value is something else";
    }
    console.log(result.next().value);

Selain itu, switch expression juga memungkinkan kamu untuk menggunakan ekspresi sebagai label case. Contohnya seperti ini:

    const value = 2;
    const result = switch (value) {
      case value > 0:
        yield "Value is positive";
      case value < 0:
        yield "Value is negative";
      default:
        yield "Value is zero";
    }
    console.log(result.next().value);

Itu hanyalah beberapa contoh dari apa yang dapat dilakukan dengan switch expression. Seperti yang bisa dilihat, switch expression memberikan cara yang lebih elegan dan ringkas untuk menuliskan kode yang berdasarkan pada nilai ekspresi tertentu. Namun, perlu diingat bahwa switch expression masih dalam tahap eksperimental dan tidak tersedia di semua browser. Jadi, sebaiknya kamu mengecek kompatibilitas browser sebelum menggunakan fitur ini dalam produksi.
