<template>
    <section>
           <!--Title-->
        <div class="container">
            <div class="contact-section">
                <h1 class="section-title">—— Restons en contact ——</h1>
                <p class="section-desc">Lorem ipsum dolor sit amet, consectetur.</p>
            </div>
        </div>
        <!--Formulaire-->
        <div class="columns contact-page">
            <div class="form column is-5-desktop is-12-mobile form-contact">
                    <!-- lien https a changé lors de la création du compte formspree -->
            <form action="https://formspree.io/xrgyynqw" method="POST">
                <h2 class="contact-title">Envoyez-nous un message</h2>
                <div class="field">
                    <label class="label" name="name">Nom</label>
                    <div class="control has-icons-left has-icons-right">
                        <input class="input" type="text" placeholder="Votre nom" name="name">
                        <span class="icon is-small is-left">
                            <i class="fa fa-user" aria-hidden="true"></i>
                        </span>
                    </div>
                </div>
                <div class="field">
                    <label class="label">Email</label>
                    <p class="control has-icons-left has-icons-right">
                        <input class="input" type="email" placeholder="Votre email" name="_replyto">
                        <span class="icon is-small is-left">
                           <i class="fa fa-envelope" aria-hidden="true"></i>
                        </span>
                    </p>
                </div>
                <div class="field">
                    <label class="label">Message</label>
                    <div class="control">
                        <textarea class="textarea" placeholder="Votre message" name="message"></textarea>
                    </div>
                </div>
                <!--Bouton-->
                <div class="btn">
                      <input class="btn-contact" type="submit" value="Envoyer">
                </div>
            </form>
            </div>
            <!--Deuxième boite-->
            <div class="column is-5-desktop is-12-mobile coord">
                <div>
                    <h2 class="contact-title">Nos coordonnées </h2>
                    <div class="contact-item">
                        <p>
                            <span class="icon is-large is-left">
                                <i class="fa fa-map-marker fa-2x mt-6" aria-hidden="true"></i>
                            </span>
                            Lorem ipsum dolor sit amet, consectetur.
                        </p>
                    </div>
                    <div class="contact-item">
                        <p>
                            <span class="icon is-large is-left">
                                <i class="fa fa-mobile fa-2x mt-6" aria-hidden="true"></i>
                            </span>
                            Lorem ipsum dolor sit amet, consectetur.
                        </p>
                    </div>
                    <div class="contact-item">
                        <p>
                            <span class="icon is-large is-left">
                                <i class="fa fa-envelope fa-2x mt-6" aria-hidden="true"></i>
                            </span>
                            Lorem ipsum dolor sit amet, consectetur.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    
    </section>
</template>

<style scoped>

.contact-page {
    justify-content: center;
}

.contact-title {
    font-family: 'Montserrat', sans-serif;
    font-size: 18px;
    font-weight: bold;
    text-align: center;
    margin-top: 5%;
    margin-bottom: 5%;
}

.contact-item {
    text-align: center;
}

.form-contact {
    margin-right: 4%;
}

@media only screen and (max-width: 1024px) {
    .form-contact {
        padding: 3%;
    }
}

@media only screen and (max-width: 769px) {
    .form-contact {
        padding: 5%;
    }
}

@media only screen and (max-width: 450px) {
    .form-contact {
        padding: 7%;
    }
}



/*boutton*/


.btn {
    text-align: center;
}

.btn-contact {
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    font-weight: bolder;
    text-transform: uppercase;
    background-color: white;
    color: #6DB6CA;
    border: 1px solid #6DB6CA;
    border-radius: 10px;
    margin-top: 3%;
    padding: 2%;
    padding-left: 3%;
    padding-right: 3%;
    cursor: pointer;
    transition: 0.5s;
}

.btn-contact:hover {
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    font-weight: bolder;
    text-transform: uppercase;
    background-color: #6DB6CA;
    color: white;
    border: 1px solid #6DB6CA;
    border-radius: 10px;
    margin-top: 3%;
    padding: 2%;
    padding-left: 3%;
    padding-right: 3%;
    cursor: pointer;
    transition: 0.5s;
}

.coord {padding-top: 3%;}

@media screen and (max-width: 1024px){

.btn{
  margin-bottom: 12rem;
}
}
</style>