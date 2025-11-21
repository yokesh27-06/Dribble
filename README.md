# Project Responsive Web Design using Bootstrap
## Date:

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Dribbble Clone - Bootstrap</title>

  <!-- Bootstrap CSS (CDN) -->
  <link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css"
    rel="stylesheet"
  />
</head>
<body class="bg-light">

  <!-- NAVBAR -->
  <nav class="navbar navbar-expand-lg border-bottom sticky-top" style="background-color: purple;">
    <div class="container">
      <a class="navbar-brand fw-bold text-white" href="#">
        dribbble<span class="text-warning">-clone</span>
      </a>
      <button class="navbar-toggler bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#mainNavbar">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="mainNavbar">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item"><a class="nav-link text-white" href="#">Inspiration</a></li>
          <li class="nav-item"><a class="nav-link text-white" href="#">Find Work</a></li>
          <li class="nav-item"><a class="nav-link text-white" href="#">Learn Design</a></li>
          <li class="nav-item"><a class="nav-link text-white" href="#">Go Pro</a></li>
        </ul>

        <form class="d-flex me-3" role="search">
          <input class="form-control form-control-sm" type="search" placeholder="Search shots">
        </form>

        <div class="d-flex align-items-center gap-2">
          <button class="btn btn-light btn-sm">Log in</button>
          <button class="btn btn-warning btn-sm">Sign up</button>
        </div>
      </div>
    </div>
  </nav>

  <!-- HERO SECTION -->
  <section class="py-5 bg-white border-bottom">
    <div class="container">
      <div class="row align-items-center gy-4">
        <div class="col-lg-6">
          <span class="badge mb-2 text-white" style="background-color: purple;">Design Inspiration</span>
          <h1 class="fw-bold mb-3">
            Discover the world’s top <span style="color: purple;">designs & shots</span>
          </h1>
          <p class="lead mb-4">
            Explore UI concepts, illustrations, branding, and more from creatives around the globe.
          </p>

          <form class="row g-2">
            <div class="col-12 col-md-8">
              <input type="text" class="form-control" placeholder="Search for UI, logo, illustration..." />
            </div>
            <div class="col-12 col-md-4 d-grid">
              <button type="submit" class="btn text-white" style="background-color: purple;">Search</button>
            </div>
          </form>
        </div>

        <div class="col-lg-6">
          <div class="card shadow-sm">
            <div class="card-body">
              <p class="text-muted small mb-2">Featured shot</p>

              <!-- UPDATED PREVIEW WITH IMAGE -->
              <div class="ratio ratio-16x9 mb-3 border">
                <img src="shot_preview.jpg" alt="Featured shot preview" style="width:100%; height:100%; object-fit:cover;">
              </div>

              <h5 class="card-title mb-1">Minimal Dashboard UI</h5>
              <p class="card-text small text-muted mb-2">by Designer Name</p>
              <div class="d-flex justify-content-between">
                <span class="small text-muted">❤ 1.2k &nbsp; 👁 10.5k</span>
                <button class="btn btn-sm text-white" style="background-color: purple;">View shot</button>
              </div>
            </div>
          </div>
        </div>

      </div>  
    </div>
  </section>

  <!-- CATEGORY TABS SECTION -->
  <section class="py-4">
    <div class="container">
      <ul class="nav nav-pills justify-content-center mb-4 flex-wrap">
        <li class="nav-item"><a class="nav-link active text-white" style="background-color: purple;" href="#">Popular</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Latest</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Web Design</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Mobile</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Branding</a></li>
      </ul>
    </div>
  </section>

  <!-- SHOTS GRID SECTION -->
<section class="pb-5">
  <div class="container">
    <div class="row g-4">

      <div class="col-12 col-sm-6 col-lg-3">
        <div class="card h-100 border-0 shadow-sm">
          <img src="shot1.jpg" class="card-img-top">
          <div class="card-body">
            <h6>E-commerce Product Page</h6>
            <span class="small text-muted">❤ 320 &nbsp; 👁 2.1k</span>
          </div>
        </div>
      </div>

      <div class="col-12 col-sm-6 col-lg-3">
        <div class="card h-100 border-0 shadow-sm">
          <img src="shot2.jpg" class="card-img-top">
          <div class="card-body">
            <h6>Food Delivery App</h6>
            <span class="small text-muted">❤ 540 &nbsp; 👁 3.7k</span>
          </div>
        </div>
      </div>

      <div class="col-12 col-sm-6 col-lg-3">
        <div class="card h-100 border-0 shadow-sm">
          <img src="shot3.jpg" class="card-img-top">
          <div class="card-body">
            <h6>Finance Dashboard</h6>
            <span class="small text-muted">❤ 780 &nbsp; 👁 5.4k</span>
          </div>
        </div>
      </div>

      <div class="col-12 col-sm-6 col-lg-3">
        <div class="card h-100 border-0 shadow-sm">
          <img src="shot4.jpg" class="card-img-top">
          <div class="card-body">
            <h6>Logo Concept</h6>
            <span class="small text-muted">❤ 190 &nbsp; 👁 1.8k</span>
          </div>
        </div>
      </div>

    </div>

    <div class="text-center mt-4">
      <button class="btn text-white" style="background-color: purple;">Load more shots</button>
    </div>
  </div>
</section>

  <!-- CALL TO ACTION -->
  <section class="py-5 bg-white border-top border-bottom text-center">
      <h2 class="fw-bold mb-3">Share your creativity with the world</h2>
      <button class="btn text-white me-2" style="background-color: purple;">Sign up free</button>
      <button class="btn btn-outline-secondary">Learn more</button>
  </section>

  <!-- FOOTER -->
  <footer class="py-3 text-center text-light" style="background-color: purple;">
      <p class="small">© 2025 Dribbble Clone (Student Project)</p>
      <p class="small">Designed by <strong>Sanjay Kumar</strong></p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

## OUTPUT:
<img width="1041" height="615" alt="image" src="https://github.com/user-attachments/assets/edeb38c1-9295-4bf2-aac8-61bd1f4c3690" />


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
