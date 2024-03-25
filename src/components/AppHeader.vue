<template>
<head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" integrity="sha512-Lx4Ln2Z0SgsNExaUeOAZlZTfS/+NDPa0T1bR1XF6XySiPf1EF3/aPuVMaNoXk1naI+8sR0ubpV0mZ8l93BlpHg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
    <nav class="navbar navbar-expand navbar-dark bg-dark">
        <a href="/" class="navbar-brand">Ứng dụng Quản lý danh bạ</a>
        <div class="mr-auto navbar-nav">
            <li class="nav-item">
                <router-link :to="{ name: 'contactbook' }" class="nav-link">
                    Danh bạ
                    <i class="fas fa-address-book"></i>
                </router-link>
            </li>
        </div>
    </nav>
</template>