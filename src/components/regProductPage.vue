<template>
    <div class="pRegister">
        <div class="title">
            <h2>Registrar novo produto:</h2>
        </div>
        <form>
            <div class="formContents">
                <div class="inptContainner">
                    <label class="label">Nome:</label>
                    <input type="text">
                    <span>Error</span>
                </div>

                <div class="inptContainner">
                    <label class="label">Categoria:</label>
                    <input type="text">
                    <span>Error</span>
                </div>

                <div class="inptContainner">
                    <label class="label">Preço:</label>
                    <input type="text">
                    <span>Error</span>
                </div>

                <div class="inptContainner inputImg">
                    <label class="label">Enviar Imagem:  <i class="fa-solid fa-file-arrow-up"></i></label>
                    <input type="file">
                    <span>Error</span>
                </div>

                <div class="inptContainner">
                    <label class="label">Nome:</label>
                    <textarea name="descrição" id="descript" cols="160" rows="10"></textarea>
                    <span>Error</span>
                </div>

                <div class="buttons">
                    <button>Cancelar</button>
                    <button>Enviar</button>
                </div>
            </div>
        </form>
    </div>
</template>

<script>
export default {
    name: "regProductPage"
};
</script>

<style scoped>
.pRegister {
    height: -webkit-fill-available;
    background-color: #F0F4FA;
    border-top: 1px solid #73777F;
}

.title h2 {
    color: #1A1C1E;
    font-size: 40px;
    margin: 24px 0 50px 21px;
}

form {
    margin: 0 21px;
}

.inptContainner {
    display: flex;
    flex-direction: column;
    width: calc(100% / 2.02);
}

.inptContainner input {
    height: 40px;
    padding-left: 10px;
    font-size: 20px;
    border-radius: 5px;
    border: 1px solid #73777f;
}

.inptContainner textarea {
    resize: none;
    padding: 10px 0 0 10px;
}

.inptContainner span {
    font-size: 12px;
    color: #ba1a1a;
}

.inputImg input[type="file"] {
    display: none;
}
.inputImg label {
    padding-top: 10px;
    height: 30px;
    width: 200px;
    background-color: #ffffff;
    border: 1px solid #73777f;
    border-radius: 5px;
    text-align: center;
    margin-top: 20px;
    cursor: pointer;
}

.fa-file-arrow-up {
    font-size: 20px;
}

.formContents {
     display: flex;
     flex-wrap: wrap;
     gap: 10px;
}

.buttons {
    width: calc(100% / 2.02);
    display: flex;
    justify-content: flex-end;
    align-items: flex-end;
    gap: 10px;
}
.buttons button {
    height: 40px;
    width: 90px;
    padding: 0 24px 0 24px;
    border-radius: 50px;
    border: none;    
}

.buttons button:first-child {
    background-color: transparent;
    color: #0062a1;
}

.buttons button:last-child {
    background-color: #0062a1;
    color: #ffffff;
}
</style>