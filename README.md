/* =========================================
   1. GOOGLE FONTS AND GLOBAL SETTINGS
========================================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

:root {
    --navy: #10243A;
    --dark-navy: #091827;
    --light-navy: #193752;
    --gold: #D4AD69;
    --white: #FFFFFF;
    --light-bg: #F4F6F8;
    --text: #263445;
    --muted: #718096;
    --border: #E1E6EC;
}

body {
    font-family: 'DM Sans', sans-serif;
    background-color: var(--white);
    color: var(--text);
    line-height: 1.7;
}

html {
    scroll-behavior: smooth;
}

a {
    text-decoration: none;
    color: inherit;
}

ul {
    list-style-position: outside;
}

.container {
    width: 88%;
    max-width: 1200px;
    margin: 0 auto;
}

section {
    scroll-margin-top: 85px;
}


/* =========================================
   2. HEADER AND NAVIGATION
========================================= */

.header {
    background-color: var(--dark-navy);
    position: sticky;
    top: 0;
    z-index: 1000;
    box-shadow: 0 3px 15px rgba(0, 0, 0, 0.12);
}

.navbar {
    min-height: 78px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-family: 'Playfair Display', serif;
    font-size: 30px;
    font-weight: 800;
    color: var(--white);
    letter-spacing: 1px;
}

.logo span {
    color: var(--gold);
}

.nav-links {
    display: flex;
    align-items: center;
    gap: 27px;
    list-style: none;
}

.nav-links a {
    color: #D9E1E9;
    font-size: 13px;
    font-weight: 500;
    transition: color 0.3s ease;
}

.nav-links a:hover {
    color: var(--gold);
}

.nav-button {
    color: var(--dark-navy);
    background-color: var(--gold);
    padding: 10px 19px;
    border-radius: 5px;
    font-size: 13px;
    font-weight: 700;
    transition: 0.3s ease;
}

.nav-button:hover {
    background-color: var(--white);
    transform: translateY(-2px);
}


/* =========================================
   3. HERO SECTION
========================================= */

.hero {
    background-color: var(--navy);
    color: var(--white);
    padding: 100px 0 110px;
    overflow: hidden;
    position: relative;
}

.hero-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 70px;
}

.hero-content {
    flex: 1.2;
}

.eyebrow,
.section-label {
    color: var(--gold);
    font-size: 12px;
    font-weight: 700;
    letter-spacing: 3px;
    margin-bottom: 18px;
}

.hero h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(42px, 5vw, 65px);
    line-height: 1.2;
    margin-bottom: 18px;
}

.hero h1 span,
.section-heading h2 span,
.contact-box h2 span {
    color: var(--gold);
}

.hero h2 {
    color: #D8E1E9;
    font-size: 19px;
    font-weight: 500;
    line-height: 1.6;
    margin-bottom: 22px;
}

.hero-description {
    color: #B8C6D3;
    max-width: 540px;
    font-size: 15px;
    margin-bottom: 30px;
}

.hero-buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 14px;
}

.btn {
    display: inline-block;
    padding: 13px 23px;
    border-radius: 5px;
    font-size: 13px;
    font-weight: 700;
    transition: all 0.3s ease;
}

.btn-primary {
    background-color: var(--gold);
    color: var(--dark-navy);
}

.btn-primary:hover {
    background-color: var(--white);
    transform: translateY(-3px);
}

.btn-outline {
    border: 1px solid #8192A3;
    color: var(--white);
}

.btn-outline:hover {
    background-color: var(--white);
    color: var(--navy);
}

.hero-location {
    color: #AAB8C7;
    margin-top: 28px;
    font-size: 13px;
}

.hero-location span {
    color: var(--gold);
    font-size: 19px;
    margin-right: 8px;
}


/* HERO IMAGE */

.hero-image {
    flex: 0.8;
    max-width: 370px;
    position: relative;
    padding: 15px;
}

.image-frame {
    height: 430px;
    width: 100%;
    border: 2px solid var(--gold);
    border-radius: 180px 180px 12px 12px;
    overflow: hidden;
    position: relative;
    z-index: 2;
    background-color: var(--light-navy);
}

.image-frame img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
}

.image-decoration {
    position: absolute;
    width: 180px;
    height: 180px;
    border: 2px solid var(--gold);
    border-radius: 50%;
    top: -15px;
    right: -25px;
    opacity: 0.6;
}

.image-caption {
    position: absolute;
    bottom: 35px;
    left: -35px;
    background-color: var(--white);
    color: var(--navy);
    padding: 14px 20px;
    border-radius: 6px;
    z-index: 3;
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.15);
}

.image-caption span {
    font-family: 'Playfair Display', serif;
    font-weight: 800;
    font-size: 22px;
    color: var(--navy);
}

.image-caption p {
    font-size: 11px;
    color: var(--muted);
}


/* =========================================
   4. GENERAL SECTION STYLING
========================================= */

.section {
    padding: 90px 0;
}

.section-heading {
    text-align: center;
    max-width: 650px;
    margin: 0 auto 50px;
}

.section-heading h2 {
    font-family: 'Playfair Display', serif;
    color: var(--navy);
    font-size: 38px;
    line-height: 1.3;
    margin-bottom: 12px;
}

.section-heading > p:last-child {
    color: var(--muted);
    font-size: 14px;
}

.section-heading .section-label {
    margin-bottom: 12px;
}


/* =========================================
   5. ABOUT SECTION
========================================= */

.about-section {
    background-color: var(--white);
}

.about-card {
    display: flex;
    gap: 35px;
    padding: 38px;
    background-color: var(--light-bg);
    border-left: 4px solid var(--gold);
    border-radius: 8px;
    margin-bottom: 35px;
}

.about-number {
    font-family: 'Playfair Display', serif;
    font-size: 45px;
    color: var(--gold);
    font-weight: 700;
}

.about-content h3 {
    font-family: 'Playfair Display', serif;
    color: var(--navy);
    font-size: 23px;
    margin-bottom: 12px;
}

.about-content p {
    color: var(--muted);
    font-size: 14px;
    line-height: 2;
}

.interest-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 22px;
}

.interest-card {
    padding: 25px;
    border: 1px solid var(--border);
    border-radius: 8px;
    transition: all 0.3s ease;
}

.interest-card:hover {
    border-color: var(--gold);
    transform: translateY(-6px);
    box-shadow: 0 8px 25px rgba(16, 36, 58, 0.08);
}

.interest-card span {
    color: var(--gold);
    font-weight: 700;
    font-size: 13px;
}

.interest-card h3 {
    color: var(--navy);
    margin: 12px 0;
    font-size: 17px;
}

.interest-card p {
    color: var(--muted);
    font-size: 13px;
}


/* =========================================
   6. EDUCATION SECTION
========================================= */

.education-section {
    background-color: var(--light-bg);
}

.education-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 25px;
}

.education-card {
    background-color: var(--white);
    border-radius: 8px;
    padding: 30px;
    border: 1px solid var(--border);
    border-top: 4px solid var(--navy);
    transition: 0.3s ease;
}

.education-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 25px rgba(16, 36, 58, 0.08);
    border-top-color: var(--gold);
}

.card-top {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 22px;
    gap: 10px;
}

.card-number {
    color: var(--gold);
    font-size: 20px;
    font-weight: 800;
}

.card-year {
    background-color: #F3EBDD;
    color: #8B6C38;
    padding: 5px 11px;
    border-radius: 20px;
    font-size: 11px;
    font-weight: 700;
}

.education-card h3 {
    color: var(--navy);
    font-size: 20px;
    line-height: 1.4;
    margin-bottom: 5px;
}

.institution-location {
    color: var(--muted);
    font-size: 12px;
}

.gold-line {
    width: 45px;
    height: 3px;
    background-color: var(--gold);
    margin: 20px 0;
}

.education-card h4 {
    color: var(--navy);
    font-size: 15px;
    margin-bottom: 10px;
}

.card-description {
    color: var(--muted);
    font-size: 13px;
    margin-bottom: 10px;
}

.education-card ul {
    padding-left: 20px;
    color: var(--muted);
    font-size: 13px;
}

.education-card li {
    margin-bottom: 7px;
}


/* =========================================
   7. EXPERIENCE SECTION
========================================= */

.experience-section {
    background-color: var(--white);
}

.experience-list {
    display: flex;
    flex-direction: column;
    gap: 24px;
}

.experience-card {
    display: grid;
    grid-template-columns: 190px 1fr;
    gap: 30px;
    padding: 32px;
    border: 1px solid var(--border);
    border-radius: 8px;
    transition: all 0.3s ease;
}

.experience-card:hover {
    border-color: var(--gold);
    box-shadow: 0 8px 25px rgba(16, 36, 58, 0.07);
    transform: translateX(5px);
}

.experience-index {
    display: block;
    font-family: 'Playfair Display', serif;
    font-size: 38px;
    font-weight: 700;
    color: var(--gold);
}

.experience-period {
    font-size: 12px;
    color: var(--muted);
    margin-top: 8px;
}

.experience-type {
    display: inline-block;
    background-color: #F3EBDD;
    color: #8B6C38;
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 1.5px;
    padding: 5px 10px;
    border-radius: 3px;
    margin-bottom: 12px;
}

.experience-right h3 {
    font-family: 'Playfair Display', serif;
    color: var(--navy);
    font-size: 22px;
    margin-bottom: 5px;
}

.experience-right h4 {
    color: var(--muted);
    font-size: 13px;
    font-weight: 500;
    margin-bottom: 17px;
}

.experience-right ul {
    padding-left: 19px;
    color: var(--muted);
    font-size: 13px;
}

.experience-right li {
    margin-bottom: 10px;
    padding-left: 4px;
}


/* =========================================
   8. SKILLS SECTION
========================================= */

.skills-section {
    background-color: var(--light-bg);
}

.skills-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 22px;
}

.skill-card {
    background-color: var(--white);
    padding: 30px;
    border-radius: 8px;
    border: 1px solid var(--border);
    transition: 0.3s ease;
}

.skill-card:hover {
    transform: translateY(-5px);
    border-color: var(--gold);
    box-shadow: 0 8px 22px rgba(16, 36, 58, 0.07);
}

.skill-icon {
    width: 42px;
    height: 42px;
    background-color: var(--navy);
    color: var(--gold);
    border-radius: 7px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 700;
    margin-bottom: 18px;
}

.skill-card h3 {
    font-family: 'Playfair Display', serif;
    font-size: 19px;
    color: var(--navy);
    margin-bottom: 15px;
}

.skill-card ul {
    padding-left: 19px;
    color: var(--muted);
    font-size: 13px;
}

.skill-card li {
    margin-bottom: 9px;
}


/* =========================================
   9. ACHIEVEMENTS SECTION
========================================= */

.achievements-section {
    background-color: var(--white);
}

.achievement-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 22px;
}

.achievement-card {
    padding: 32px 20px;
    text-align: center;
    background-color: var(--navy);
    border-radius: 8px;
    color: var(--white);
    transition: 0.3s ease;
}

.achievement-card:hover {
    transform: translateY(-7px);
    background-color: var(--dark-navy);
}

.achievement-symbol {
    color: var(--gold);
    font-size: 30px;
    font-weight: 700;
    margin-bottom: 15px;
}

.achievement-card h3 {
    font-family: 'Playfair Display', serif;
    font-size: 23px;
    margin-bottom: 8px;
}

.achievement-card p {
    color: #D9E1E9;
    font-size: 14px;
}

.achievement-card span {
    display: block;
    color: #AAB8C7;
    font-size: 11px;
    margin-top: 12px;
}


/* =========================================
   10. CONTACT SECTION
========================================= */

.contact-section {
    background-color: var(--light-bg);
}

.contact-box {
    background-color: var(--navy);
    padding: 65px 45px;
    border-radius: 10px;
    text-align: center;
    color: var(--white);
}

.contact-box h2 {
    font-family: 'Playfair Display', serif;
    font-size: 38px;
    margin-bottom: 18px;
}

.contact-description {
    max-width: 580px;
    margin: 0 auto 35px;
    color: #B8C6D3;
    font-size: 14px;
}

.contact-details {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 40px;
    margin-bottom: 35px;
}

.contact-item {
    text-align: center;
}

.contact-label {
    display: block;
    color: var(--gold);
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 2px;
    margin-bottom: 7px;
}

.contact-item a,
.contact-item p {
    color: var(--white);
    font-size: 13px;
}

.contact-item a:hover {
    color: var(--gold);
}

.btn-gold {
    background-color: var(--gold);
    color: var(--dark-navy);
}

.btn-gold:hover {
    background-color: var(--white);
    transform: translateY(-3px);
}


/* =========================================
   11. FOOTER
========================================= */

.footer {
    background-color: var(--dark-navy);
    padding: 25px 0;
}

.footer-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 20px;
}

.footer-content p {
    color: #AAB8C7;
    font-size: 11px;
}


/* =========================================
   12. RESPONSIVE DESIGN - TABLETS
========================================= */

@media screen and (max-width: 900px) {

    .navbar {
        flex-wrap: wrap;
        padding: 15px 0;
        gap: 15px;
    }

    .nav-links {
        gap: 15px;
        flex-wrap: wrap;
        justify-content: center;
    }

    .hero-container {
        gap: 35px;
    }

    .hero h1 {
        font-size: 45px;
    }

    .hero-image {
        max-width: 300px;
    }

    .image-frame {
        height: 360px;
    }

    .experience-card {
        grid-template-columns: 130px 1fr;
    }

}


/* =========================================
   13. RESPONSIVE DESIGN - MOBILE
========================================= */

@media screen and (max-width: 600px) {

    .container {
        width: 90%;
    }

    .section {
        padding: 65px 0;
    }

    .navbar {
        justify-content: center;
    }

    .logo {
        width: 100%;
        text-align: center;
    }

    .nav-links {
        gap: 12px 18px;
    }

    .nav-links a {
        font-size: 11px;
    }

    .nav-button {
        display: none;
    }

    .hero {
        padding: 65px 0;
    }

    .hero-container {
        flex-direction: column-reverse;
        text-align: center;
    }

    .hero-content {
        width: 100%;
    }

    .hero h1 {
        font-size: 40px;
    }

    .hero h2 {
        font-size: 16px;
    }

    .hero-description {
        font-size: 13px;
    }

    .hero-buttons {
        justify-content: center;
    }

    .hero-location {
        margin-top: 20px;
    }

    .hero-image {
        width: 80%;
        max-width: 280px;
    }

    .image-frame {
        height: 330px;
    }

    .image-caption {
        left: -15px;
    }

    .section-heading h2 {
        font-size: 30px;
    }

    .about-card {
        flex-direction: column;
        gap: 10px;
        padding: 25px;
    }

    .about-number {
        font-size: 32px;
    }

    .interest-grid,
    .education-grid,
    .skills-grid,
    .achievement-grid {
        grid-template-columns: 1fr;
    }

    .experience-card {
        grid-template-columns: 1fr;
        gap: 15px;
        padding: 24px;
    }

    .experience-index {
        font-size: 28px;
    }

    .experience-right h3 {
        font-size: 19px;
    }

    .contact-box {
        padding: 40px 20px;
    }

    .contact-box h2 {
        font-size: 29px;
    }

    .contact-details {
        flex-direction: column;
        gap: 22px;
    }

    .footer-content {
        flex-direction: column;
        text-align: center;
    }

}


/* =========================================
   14. SMALL SCREEN ADJUSTMENTS
========================================= */

@media screen and (max-width: 380px) {

    .hero h1 {
        font-size: 34px;
    }

    .nav-links {
        gap: 10px;
    }

    .nav-links a {
        font-size: 10px;
    }

    .btn {
        padding: 11px 15px;
        font-size: 11px;
    }

}
