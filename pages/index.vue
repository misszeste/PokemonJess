<style>
.mb3{   
    margin-left: 25%;
    margin-right: 25%;
    margin-bottom: 08%;
    align-self: center;
}
</style>
<template>    
        <h2 style="text-align:center">Se connecter pour visualiser la liste</h2>  
        <div class="mb3">
            <form style="padding:8%">                
                <div class="row mb-3">
                    <label for="inputEmail3" class="col-sm-2 col-form-label"><b>Courriel</b></label>
                    <div class="col-sm-10">
                    <input type="email" class="form-control" id="inputEmail3">
                    </div>
                </div>
                <div class="row mb-3">
                    <label for="inputPassword3" class="col-sm-2 col-form-label"><b>Mot de passe</b></label>
                    <div class="col-sm-10">
                    <input type="password" class="form-control" id="inputPassword3">
                    </div>
                </div>
                    <div class="row mb-3">
                    <div class="col-sm-10 offset-sm-2">
                    <div class="form-check">
                        <input class="form-check-input" type="checkbox" id="gridCheck1">
                        <label class="form-check-label" for="gridCheck1"><b>
                            Se souvenir de moi
                        </b></label>
                    </div>
                    </div>
                </div>
                <div style="padding-top:8%">
                    <button type="submit" class="btn btn-primary">Se connecter</button>
                    
                </div>
                
            </form>
        </div>
</template>
