# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...



1. un utilisateur est cree en bdd par le model 
2. grace au calback  after_create, on execute la methode welcomw_send sur l'instance qui vient detre sauvee en bdd
3. welcome dit en resume execute now la methode welcome_email situe dans le userMailer
4. wecolme_email va apeler 2 template en leur mettant a disposition une instance @user qui est l'utilisateur cree et une variable @url qui est juste une string. Cette methode enverra ensuite les 2 templates @user.email avec comme sujet "Bienvenue chew nous
5.  les 2 templates (un html et un text) sont personalise avec les entree en Ruby (@user.name, @user.email et @url avant detre balance par mail)
# test_action_mailer_send_grid
# test_action_mailer_send_grid
