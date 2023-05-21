-------CSS code with notes.-------
<br>
-------Código css com comentários.-------


*{ /*é bom formatar margin e padding para 0*/
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body, input, button, select, textarea{
    font-family: 'Poppins', sans-serif;
    background: #E5E5E5;

}

/*o ::before significa que ele vai ficar antes de um conteúdo! z-index: significa a opsição de camada que ele vai ficar*/
body::before{
    content: '';
    width: 100%;
    height: 368px;
    
    position:absolute;
    top: 0;
    left: 0;
    z-index: -1;
    background: #121214;
}

.page{
    width: 736px;
    margin: auto;
}

header{
    width: 319px;
    margin-top: 74px;
}

header h1{
    font-family: 'Archivo', sans-serif;
    font-weight: bold;
    color: white;
    font-size: 36px;
    line-height: 42px;

    margin-bottom: 24px;
}
header p{
    font-style: normal;
    color: #42D3FF;
    font-size: 16px;
    line-height: 26px;
}

form{
    background: #fafafc;
    border-radius: 8px 8px 0 0;

    margin-top: 38px;
    min-height: 300px;
    padding: 64px;


    /*para aplicar um padrão de distancia entre os elementos*/
    display: flex;
    flex-direction: column;
    gap: 48px;
}

fieldset{
    border: none;
}

.fieldset-wrapper{
    
    display:flex;
    flex-direction: column;
    gap: 24px;
}

fieldset legend{
    font-family: 'Archivo';
    font-weight: 600;
    font-size: 24px;
    line-height: 34px;
    width: 100%;
    border-bottom: 1px solid #E6E6F0;
    padding-bottom: 16px;
}

.input-wrapper{
    display: flex;
    flex-direction: column;
}
.input-wrapper label, .pretty p-icon p-round p-smooth{
    font-size: 14px;
    line-height: 24px;

    color: #4E4958;

    margin-bottom: 8px;
}



.input-wrapper span:hover{
    color: #6c6972;
}
.input-wrapper label span{
    margin-left: 12px;
    font-size: 12px;
    line-height: 20px;
    color: #C1BCCC;
}
.input-wrapper input, .input-wrapper textarea, .input-wrapper select{
    background: #FAFAFC;

    border: 1px solid #E6E6F0;
    /*box-sizing: border-box; calculo do tamanho da caixa| o tamanho da caixa vai ser em relação a borda*/
    border-radius: 8px; 
    
    padding: 0 24px;
    height: 56px;

    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 26px;
    
    color: #C1BCCC;
    
}

.input-wrapper textarea{
    height: 168px;
    padding: 0;
}

.input-wrapper select{
    appearance: none; /*tira a setinha para baixo do select*/
}
.input-wrapper select:hover{
    background: #E5E5E5;
}
.input-wrapper option:hover{
    background: #E5E5E5;
}
.colunas{
    display: flex;
    gap: 20px;
}
/*ordena niveis de algo nesse caso uma div*/
.colunas > div:nth-child(1){
    width: 100%;
    
}
.pretty p-icon p-round p-smooth{
    position: relative;
}
.pretty p-icon p-round p-smooth label{
    display:flex;
    align-items: center;
    gap: 16px;
    cursor: pointer;
}
.pretty p-icon p-round p-smooth input{
    /*display:none; usa o display:none para sumir com a caixa de seleção
                    para poder configurar ele, senão sempre vai ficar pegando a caixinha do navegador*/
    position: absolute;
    top: 0;
    left: 0;
}
.pretty p-icon p-round p-smooth label::before{
    content: '';
    width: 24px;
    height: 24px;
    display: block;

    border: 1px solid #E6E6F0;
    border-radius: 8px;
}
.pretty p-icon p-round p-smooth:focus + label::before{
    outline: 2px solid black;
}
footer{
    height: 136px;

    background: #f0f0f4;
    
    display:flex;
    flex-direction: column;

    padding: 40px 64px;

    border-top: 1px solid #d6d6d6;
    border-radius: 0 0 8px 8px;
}

footer .button{
    height: 56px;
    background-color: #04d361;
    border-radius: 8px;
    border: 0;

    font-weight: 600;
    font-size: 16px;
    line-height: 26px;
}
footer .button:hover{
    background-color: #02b050;

}

input:invalid{
    border: 1px solid #ff1010;
}
