<html>
  <meta charset="UTF-8" /><meta
    content="width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5"
    name="viewport"
  /><meta content="IE=edge" http-equiv="X-UA-Compatible" />
  <link rel="preconnect" href="https://fonts.googleapis.com" /><link
    rel="preconnect"
    href="https://fonts.gstatic.com"
    crossorigin
  /><link
    href="https://fonts.googleapis.com/css2?family=Quicksand&display=swap"
    rel="stylesheet"
  />
  <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script>
  <link
    href="https://hanyauntukmu.likeadream.repl.co/style.css"
    rel="stylesheet"
    type="text/css"
  />
  <script src="https://hanyauntukmu.likeadream.repl.co/script.js"></script>
  <head> 
    <title> Hello :D</title>
  </head>
  <style>
    body {
      background-image: url(https://i.postimg.cc/DyDxMt8v/pexels-photo-8489373.jpg);
      background-repeat: no-repeat;
      background-size: cover;
      background-position-y: bottom;
    }
    body::before {
      content: "" !important;
      color: transparent !important;
    }
  </style>
  <body>
    <div id="bodyblur">
      <!-- <img
        src="https://i.postimg.cc/DyDxMt8v/pexels-photo-8489373.jpg"
        width="100%"
        height="100%"
      /> -->
    </div>

    <div id="Content">
      <div class="image">
        <img
          src="https://i.postimg.cc/qMRgtdyv/b49009850e788a06c5be434feae580b9.gif"
          width="130px"
          height="130px"
        />
      </div>
      <div>
        <blockquote>
          <p id="text"></p>
          <p id="text2"></p>
        </blockquote>
      </div>
    </div>

    <script type="text/javascript">
      function play() {
        var audio = new Audio(
          "https://sndup.net/tqdx/d"
        )
        audio.play()
      }

      const swals = Swal.mixin({
        allowOutsideClick: false,
        cancelButtonColor: "black",
      })
      const swalsy = Swal.mixin({
        confirmButtonText: "Iya",
        allowOutsideClick: false,
      })
      const swalst = Swal.mixin({
        allowOutsideClick: false,
        showConfirmButton: false,
        timer: 8000,
        timerProgressBar: true,
      })

      async function mulaitanya() {
        var { isConfirmed: tanyawal } = await swals.fire({
          title: `Klik ya, aman. orane saldo m-bankinge ilang`,
          imageUrl: "https://i.postimg.cc/jSgK0VmG/d929643638ed083a1b5c169ae95aef28.gif",
          imageWidth: 120,
          imageHeight: 120,
          confirmButtonText: "Okay",
          allowOutsideClick: false,
          showCancelButton: false,
         })
        if (tanyawal) {
          play()
          kuis()
        }
      }

      async function kuis() {
        await swalst.fire({
          title: "Gimana hari ini? capek ya? (:",
          imageUrl: "https://i.postimg.cc/02wF21b1/peach-goma.gif",
          imageWidth: 120,
          imageHeight: 120,
        })
        await swalst.fire({
          title: "Its okay, selamat ya udah bisa ngelewatin semua hal dihari ini",
          imageUrl: "https://i.postimg.cc/g06FWScx/tepukbadan.gif",
          imageWidth: 120,
          imageHeight: 120,
        })
        await swalst.fire({
          title: " Ojo lali maem ...",
          imageUrl: "https://i.postimg.cc/Dfcn7bXV/bear-panda.gif",
          imageWidth: 120,
          imageHeight: 120,
        })
        await swalst.fire({
          title: "Istirahaat, biar ilang capeknya...",
          imageUrl: "https://i.postimg.cc/SsmkcNY9/bear-cute-1.gif",
          imageWidth: 120,
          imageHeight: 120,
        })
        text = " hehehe...   Jaga diri baik-baik, tetep semangat "
        showDiv()
      }
      mulaitanya()
    </script>
  </body>
</html>
