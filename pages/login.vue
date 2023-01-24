import { defineNuxtConfig } from 'nuxt3'

<!-- Standard pour la structure -->
<template>
    <h2 style="text-align:center">Inscrivez-vous pour visualiser la liste</h2>  
    <div class="mb3" style="padding-top:3%">            
            <form class="row g-3">
                <div class="col-md-6">
                    <label for="inputEmail4" class="form-label"><b>Courriel</b></label>
                    <input type="email" class="form-control" id="inputEmail4">
                </div>
                <div class="col-md-6">
                    <label for="inputPassword4" class="form-label"><b>Mot de passe</b></label>
                    <input type="password" class="form-control" id="inputPassword4">
                </div>
                <div class="col-12">
                    <label for="inputAddress" class="form-label"><b>Adresse</b></label>
                    <input type="text" class="form-control" id="inputAddress" placeholder="123 Rue des souvenirs">
                </div>
            
                <div class="col-md-6">
                    <label for="inputCity" class="form-label"><b>Ville</b></label>
                    <input type="text" class="form-control" id="inputCity">
                </div>
                <div class="col-md-4">
                    <label for="inputState" class="form-label"><b>Province</b></label>
                    <select id="inputState" class="form-select">
                        <option selected>Québec</option>
                        <option>Alberta</option>
                        <option>Colombie Britanique</option>                  
                        <option> Île-du-Prince-Édouard </option>
                        <option value="">Manitoba</option>
                        <option value="">Nouveau-Brunswick</option>
                        <option value="">Nouvelle-Écosse</option>
                        <option value="">Nunavut</option>
                        <option>Ontario</option>
                        <option value="">Saskatchewan</option>
                        <option value="">Terre-Neuve-et-Labrador</option>
                        <option value="">Territoires du Nord-Ouest</option>
                        <option value="">Yukon</option>
                    </select>
                </div>
                <div class="col-md-2">
                    <label for="inputCP" class="form-label"><b> Postal</b></label>
                    <input type="text" class="form-control" id="inputCP">
                </div>
                <div>
                    <div class="col-12">
                        <div class="form-check">
                        <input class="form-check-input" type="checkbox" id="gridCheck">
                        <label class="form-check-label" for="gridCheck"><b>
                            Se souvenir de moi
                        </b></label>
                        </div>
                    </div>
                    <div class="col-12" style="padding-top:8%">
                        <button type="submit" class="btn btn-primary">S'enregistrer</button>
                    </div>
                </div>
            </form>
        </div>    
</template>