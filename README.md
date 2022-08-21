.header {
    background-image: linear-gradient(0, #fe6533, #f63f2e);
    height: var(--header-height);
}

.header__navbar {
    display: flex;
    justify-content: space-between;
}

.header__navbar-list {
    list-style: none;
    padding-left: 0;
    margin: 4px 0 0 0;
    display: flex;
    text-align: center;
}   

.header__navbar-icon-link {
    color: var(--white-color);
    text-decoration: none;
   
}

.header__navbar-icon-link:nth-child(2) {
    margin-left: 2px;
}

.header__navbar-item {
    margin: 0 8px;
    position: relative;
    min-height: 26px;
    
}

.header__navbar-user {
    display: flex;
    justify-items: center;
    position: relative;
}

.header__navbar-user-img {
    width: 22px;
    height: 22px;
    border-radius: 50%;
    border: 1px solid rgba (0, 0, 0, 0.1)
    
}




.header__navbar-user-name {
    margin-left: 4px;
    font-size: 1.4rem;
    font-weight: 400;
    color: var(--white-color);
}

.header__navbar-user-item {
    padding: 3px;
    display: flex;  
}
.header__navbar-user-menu {
    position: absolute;
    padding-left: 0;
    top: 40px;
    right: 40px;
    background-color: var(--white-color);
    border-radius: 2px;
    width: 160px;
    z-index: 1; 
    list-style: none;
    box-shadow: 0 1px 2px #e0e0e0;
    display: none;
}

.header__navbar-user-item--separate {
    border-top: 1px solid rgba(0, 0, 0, 0.05);
}

.header__navbar-user:hover .header__navbar-user-menu {
    display: block;
}

.header__navbar-user-menu::before {
    content: "";
    border-width: 19px 15px;
    border-style: solid;
    border-color: transparent transparent var(--white-color) transparent;
    position: absolute;
    right: 4px;
    top: -38px;


}

.header__navbar-user-item {

}
.header__navbar-user-item a {
    text-decoration: none;
    color: var(--text-color);
    font-size: 1.4rem;
    padding: 4px 16px;
    
}

.header__navbar-user-item a:hover {
    background-color: red;

}

.header__navbar-item--has-notify:hover .header__notify {
    display: block;

}

.header__navbar-item, 
.header__navabar-item-link {
    display: inline-block;
    font-size: 1.3rem;
    color: var(--white-color);
    font-weight: 300;
    text-decoration: none;
}

.header__navbar-item, 
.header__navabar-item-link,
.header__navbar-icon-link {
    display: flex;
    align-items: center;
}

.header__navbar-item:hover, 
.header__navbar-icon-link:hover,
.header__navabar-item-link:hover {
    color: rgba(255, 255, 255, 0.7);
    cursor: pointer;
    z-index: 1;
}

.header__navabr-item-link--strong {
    font-weight: 400;
}

.header__navbar-item--separate::after {
    content: "";
    display: block;
    position: absolute;
    border-left: 1px solid #fb9086;
    height: 16px;
    right: -9px;
    top: 50%;
    transform: translateY(-50%);
}

.header__navbar-icon {
    font-size: 1.8rem;
    margin: 0 4px;
    
}

.header__navbar--title-no-pointer {
    cursor: text;
    color: var(--white-color);
}
/* Heder QR code */
.header__qr {
    background-color: var(--white-color);
    width: 186px;
    position: absolute;
    left: 0;
    top: 118%;
    padding: 8px;
    border-radius: 2px;
    display: none;
    animation: fadeIn ease-in 0.3s;
    
}
.header__qr::before{
    position: absolute;
    width: 100%;
    top: -16px;
    left: 0;
    height: 20px;
    content: "";
    display: block;
    

}
.header__qr-img {
    width: 100%;
}

.header__qr-apps {
    display: flex;
    justify-content: space-between;
}


.header__qr-dowload-img {
    height: 16px;
}

.header__qr_link:nth-child(1) {
    margin-left: 11px;
}


.header__qr_link:nth-child(2) {
    margin-right: 11px;
}

.header__navbar-item--has-qr:hover .header__qr  {
    display: block;
}
 

/* Header Notify */

.header__notify {
    position: absolute;
    top: 118%;
    width: 404px;
    border-radius: 2px;
    background-color: var(--white-color);
    right: 0;
    border: 1px solid rgba(0, 0, 0, 0.1);
    cursor: default;
    animation: headerNotifyGrowth ease-in 0.2s;
    transform-origin: calc(100% - 32px) top;
    will-change: opacity, transform;
    display: none;
    
}
@keyframes headerNotifyGrowth {
    from {
        opacity: 0;
        transform: scale(0);
    }

    to {
        opacity: 1;
        transform: scale(1);
    }
}

.header__notify::before {
    content: "";
    border-width: 20px 27px;
    border-style: solid;
    border-color: transparent transparent var(--white-color) transparent;
    position: absolute;
    right: 4px;
    top: -29px;


}
.header__notify::after {
    content: "";
    display: block;
    position: absolute;
    right: 0;
    top: -16px;
    width: 90px;
    height: 20px;

}



.header__notify-header {
    height: 40px;
    display: flex;   
    background-color: var(--white-color);

}

.header__notify-header  h3 {
    color: #999;
    margin: 0 0 0 12px;
    font-weight: 400;
    font-size: 1.4rem;
    line-height: 40px;
    user-select: none;
}

.header__notify-list {
    
}

.header__notify-item {
    display: flex;
}

.header__notify-item:hover {
    background-color: #f7f7f7;
}

.header__notify-item--viewed {
    background-color: rgba(238, 75, 43, 0.08);

}

.header__notify-link {
    display: flex;
    width: 100%;
    padding: 12px;   
    text-decoration: none;
}


.header__notify-img {
    width: 48px;
    object-fit: contain;
}

.header__notify-info {
    margin-left: 12px;
}

.header__notify-name {
    display: block;
    font-size: 1.4rem;
    color: var(--text-color);
    font-weight: 400;
    line-height: 1.8rem;
}

.header__notify-descrition {
    display: block;
    font-size: 1.2rem;
    line-height: 1.6rem;
    color: #756f6e;
    margin-top: 4px;
}

.header__notify-footer {
    display: flex;
}

.header__notify-footer--btn {
    text-decoration: none;
    color: var(--text-color);
    padding: 8px 0;
    width: 100%;
    margin: auto;
    font-size: 1.4rem;
    font-weight: 400;
    text-align: center;
}

/* Authen modal */
.auth-form {
    width: 500px;
    background-color: var(--white-color);
    border-radius: 5px;
    overflow: hidden;
}

.auth-form__container {
    padding: 0 32px;

}
.auth-form__header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 12px;
    margin-top: 10px;
}
.auth-form__heading {
    font-size: 2.2rem;
    font-weight: 400;
    color: var(--text-color);
}
.auth-form__switch-btn {
    font-size: 1.6rem;
    font-weight: 400;
    color: var(--primary-color);
    cursor: pointer;
}
.auth-form__input {
    width: 100%;
    height: 40px;
    margin-top: 16px;
    padding: 0 12px;
    font-size: 1.4rem;
    border: 1px solid var(--border-color);
    border-radius: 2px;
    outline: none;
}

.auth-form__input:focus {
    border-color: #888;
}
.auth-form__form {
   
}

.auth-form__aside {
    margin-top: 18px;
}
.auth-form__policy-text {
    font-size: 1.3rem;
    line-height: 1.6rem;
    text-align: center;
    padding: 0 12px;
}
.auth-form__text-link {
    text-decoration: none;
    color: var(--primary-color);
}
.auth-form__controls {
    margin-top: 80px;
    display: flex;
    justify-content: flex-end;

}
.auth-form__socials {
   background-color: #f5f5f5;
   padding: 16px 36px;
   display: flex;
   justify-content: space-between;
   margin-top: 22px;
   
}
.auth-form__controls-back {
    margin-right: 8px;
    background-color: var(--while-color);
}


.btn--with-icons {
    padding-left: 28px;
}

/* Selection */

.select-input {
    height: 34px;
    padding: 0 12px;
    border-radius: 2px;
    background-color:var(--white-color);
    min-width: 200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
}

.select-input__label {
    font-size: 1.4rem;
    
}

.select-input__icon {
    font-size: 1.4rem;
    color: rgba(131, 131, 131);
    position: relative;
    top: 1px;
}

.select-input__list {
    position: absolute;
    left: 0;
    right: 0;
    top: 25px;
    border-radius: 2px;
    background-color: var(--white-color);
    padding: 8px 16px;
    list-style: none;
    display: none;
}

.select-input:hover .select-input__list{
    display: block;
} 

.select-input__link {
    font-size: 1.2rem;
    color: var(--text-color);
    text-decoration: none;
    display: block;
    padding: 4px 0;

}

.select-input__link:hover {
    color: var(--primary-color);

}


