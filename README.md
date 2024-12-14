<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Demo Website 1</title>
  <!-- Google Tag Manager Snippet -->
  <script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
  new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
  j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
  'https://www.googletagmanager.com/gtm.js?id=' + i + dl;f.parentNode.insertBefore(j,f);
  })(window,document,'script','dataLayer','GTM-PBRG3HBL');</script>
</head>
<body>
  <header>
    <h1>Welcome to Demo Website 1</h1>
  </header>

  <main>
    <p>This is a demo page to test cross-domain tracking.</p>

    <!-- Cross-domain link -->
    <a href="https://your-second-domain.github.io" id="crossDomainLink">Go to Demo Website 2</a>

    <!-- Add to Cart Button -->
    <div>
      <button id="addToCartButton">Add to Cart</button>
    </div>
  </main>

  <script>
    // Simulating an Add to Cart event
    document.getElementById("addToCartButton").addEventListener("click", function () {
      console.log("Add to Cart button clicked");
      // You can use GTM to capture this event and send it to GA4
      alert("Item added to cart!");
    });

    // Tracking click on the cross-domain link
    document.getElementById("crossDomainLink").addEventListener("click", function () {
      console.log("Navigating to another domain");
      // Linker or tracking via GTM will handle session continuation
    });
  </script>
</body>
</html>
