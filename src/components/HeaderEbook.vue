<template>
    <header class="header-area header-ebook navbar-light" :class="{'is-sticky': isSticky}">
        <div class="container-fluid container-fluid--cp-150">
            <nav class="navbar navbar-expand-lg" id="navbar-example2">
                <router-link to="/">
                    <img src="../assets/img/logo/logo-dark.png" alt="logo">
                </router-link>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>

                <div class="collapse navbar-collapse justify-content-center" id="navbarSupportedContent">
                    <ul class="nav main-menu">
                        <li class="nav-item">
                            <a class="nav-link" href="#home" @click="menuCollapseOnLinkClick">
                                <span>HOME</span>
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#intro" @click="menuCollapseOnLinkClick">
                                <span>Mega Ace Hackathon</span>
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#whitepaper" @click="menuCollapseOnLinkClick">
                                <span>Whitepaper</span>
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#faq" @click="menuCollapseOnLinkClick">
                                <span>MVP on testnet</span>
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#faq" @click="menuCollapseOnLinkClick">
                                <span>FAQ</span>
                            </a>
                        </li>
                    </ul>
                </div>
            </nav>
        </div>
    </header>
</template>

<script>
    export default {
        data (){
            return {
                isSticky: false,
            }
        },

        mounted(){
            window.addEventListener('scroll', () => {
                let scroll = window.scrollY
                if(scroll >= 200){
                    this.isSticky = true
                } else {
                    this.isSticky = false
                }
            })
        },

        methods: {
            // offcanvas searchbox
            toggleClass(addRemoveClass, className) {
                const el = document.querySelector('#search-overlay');
                if (addRemoveClass === 'addClass') {
                    el.classList.add(className);
                } else {
                    el.classList.remove(className);
                }
            },
            menuCollapseOnLinkClick() {
                document.getElementById('navbarSupportedContent').classList.remove('show')
            }
        },
    }
</script>

<style lang="scss" scoped>
    .header-ebook {
        &.is-sticky {
            top: 0;
            left: 0;
            position: fixed;
            width: 100%;
        }
    }
</style>