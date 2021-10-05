<template>
    <div>
        <div>
            <form id="Form">
                <!-- Cliente -->
                <div class="input-container">
                    <label for="nome">Nome do Cliente</label>
                    <input type="text" id="nome" name="name" v-model="nome" placeholder="Digite o seu nome">
                </div>
                <!-- Recipiente -->
                <div class="input-container">
                    <label for="recipíente" id="recipiente">Escolha o recipiente do sorvete:</label>
                    <select name="recipíente" id="recipiente" v-model="recipiente">
                        <option value=""></option>
                        <option value="casquinha">Casquinha</option>
                    </select>  
                </div>
                <!-- Sabor -->
                <div>
                    <div class="input-container">
                        <label for="sabor" id="sabor">Escolha o sabor do sorvete:</label>
                            <select name="sabor" id="sabor" v-model="sabor">
                                <option value=""></option>
                                <option value="baunilha">Baunilha</option>
                            </select>  
                    </div>
                </div>
                <!-- Opcionais -->
                <div>
                    <div id="opcionais-container" class="input-container">
                        <label id="opcionais-title" for="opcionais">Quer adicionar alguns opcional :</label>
                            <div class="checkbox-container">
                            <input type="checkbox" name="opcionais" v-model="opcionais" value="confete">
                                <span>Confete</span>
                            </div>
                            <div class="checkbox-container">
                            <input type="checkbox" name="opcionais" v-model="opcionais" value="confete">
                                <span>Chantily</span>
                            </div>
                            <div class="checkbox-container">
                            <input type="checkbox" name="opcionais" v-model="opcionais" value="confete">
                                <span>Canudinho</span>
                            </div>
                            <div class="checkbox-container">
                            <input type="checkbox" name="opcionais" v-model="opcionais" value="confete">
                                <span>Granulado</span>
                            </div>
                    </div>  
                </div>
            </form>
        </div>
        <div class="input-container">
            <input type="submit" class="submit-btn" value="Criar meu sorvete !">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Form'
    }
</script>

<style>
    #Form {
        max-width: 400px;
        margin: 0 auto;
    }

    .input-container {
        display: flex;
        flex-direction: column;
        margin-bottom: 20px;
    }

    label {
        font-weight: bold;
        margin-bottom: 15px;
        color: #DB4D89;
        padding: 5px 10px;
        border-left:4px solid #9FD9FF ;
    }

    input, select {
        padding: 5px 10px;
        width: 300px;
    }

    #opcionais-container {
        flex-direction: row;
        flex-wrap: wrap;
    }

    #opcionais-title {
        widows: 100%;
    }

    .checkbox-container {
        display: flex;
        align-items: flex-start;
        width: 50%;
        margin-bottom: 20px;
    }

    .checkbox-container span,
    .checkbox-container input {
        width: auto;
    }

    .checkbox-container span {
        margin-left: 6px;
        font-weight: bold;
    }

    .submit-btn {
        background-color: #DB4D89;
        color: #9FD9FF;
        font-weight: bold;
        border: 2px solid #9FD9FF;
        padding: 10px;
        font-size: 16px;
        margin: 0 auto;
        cursor: pointer;
        transition: .5s;
    }

    .submit-btn:hover {
        background-color: transparent;
        color: violet;
    }
</style>
