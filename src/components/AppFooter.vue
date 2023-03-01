<template>
    <footer class="main-footer">
        <div class="footer-sidebar">
            <div class="container">
                <div class="card">
                    <div class="card-img">
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="card-body">
                        <p>digital comics</p>
                    </div>
                </div>
                <div class="card">
                    <div class="card-img">
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="card-body">
                        <p>digital comics</p>
                    </div>
                </div>
                <div class="card">
                    <div class="card-img">
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="card-body">
                        <p>digital comics</p>
                    </div>
                </div>
                <div class="card">
                    <div class="card-img">
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="card-body">
                        <p>digital comics</p>
                    </div>
                </div>
                <div class="card">
                    <div class="card-img">
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="card-body">
                        <p>digital comics</p>
                    </div>
                </div>
            </div>

        </div>
        <div class="footer-links">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div class="menu">
                            <h2 class="menu-title">dc comics</h2>
                            <ul>
                                <li class="menu-item">link</li>
                                <li class="menu-item">link</li>
                                <li class="menu-item">link</li>
                                <li class="menu-item">link</li>
                                <li class="menu-item">link</li>
                                <li class="menu-item">link</li>
                            </ul>
                        </div>

                        <div>
                            <h2 class="menu-title">dc comics</h2>
                            <ul>
                                <li class="menu-item">link</li>
                                <li class="menu-item">link</li>
                            </ul>
                        </div>
                    </div>

                    <div class="col">
                        <h2 class="menu-title">dc comics</h2>
                        <ul>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                        </ul>
                    </div>

                    <div class="col">
                        <h2 class="menu-title">dc comics</h2>
                        <ul>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                            <li class="menu-item">link</li>
                        </ul>
                    </div>
                </div>
                <div class="col">
                    <img src="/img/dc-logo-bg.png" alt="Dc Logo">
                </div>
            </div>
        </div>

        <div class="footer-social">

            <div class="container">
                <button class="btn btn-sign">sign-up now!</button>
                <div class="social-wrap">
                    <button class="btn btn-follow">follow us</button>
                    <img src="/img/footer-facebook.png" alt="">
                    <img src="/img/footer-twitter.png" alt="">
                    <img src="/img/footer-youtube.png" alt="">
                    <img src="/img/footer-pinterest.png" alt="">
                    <img src="/img/footer-periscope.png" alt="">

                </div>
            </div>

        </div>
    </footer>
</template>
  
<script>

</script>
  
<style scoped>
.main-footer {
    color: white;
}

.container {
    justify-content: space-between;
    padding: 10px;
}

.footer-sidebar {
    background-color: #0282f9;
    padding: 20px;
    position: relative;
    z-index: 999;
}

.card {
    padding: 20px;
    display: flex;
    align-items: center;
    gap: 10px;
}

.card-img img {
    height: 30px;
}

.footer-links {
    background-image: url('/img/footer-bg.jpg');
    background-size: cover;
    padding: 20px;
    color: white;
    height: 260px;
}

.row {
    display: flex;
    gap: 15px;
}

.menu {
    margin-bottom: 10px;
}

.menu-title {
    text-transform: uppercase;
    font-size: 15px;
    margin-bottom: 10px;
}

.menu-item {
    font-size: 12px;
    font-weight: 700;
    color: #837f77;
}

.col img {
    height: 400px;
    position: relative;
    bottom: 100px;
}

.footer-social {
    background-color: #303030;
    padding: 20px;
    position: relative;
    z-index: 999;
}

.btn {
    text-transform: uppercase;
    padding: 10px;
    font-weight: 700;
}

.btn-sign {
    background-color: unset;
    border: 2px solid #0282f9;
    color: white;
    font-size: 12px;
}

.social-wrap {
    display: flex;
    align-items: center;
    gap: 20px;
}

.btn-follow {
    background-color: unset;
    color: #0282f9;
    border: none;
}
</style>