# Android: GPS com Google Maps

1. Criar um projeto novo. Meu projeto irá chamar `Android_GPS_23_06_2021`
2. Selecionar `Google Maps Activity`
   - ![Criação do Projeto](Criacao_Projeto.png)
   - Aguardar indexar e dar `play` na aplicação.

## Configuração e criação da Chave de Api do Google Maps

1. Certifique-se de que está com o arquivo `google_maps_api.xml` aberto.

2. Procure pelo link que começa com `https://console.developers.google.com/flows/`, geralmente é o primeiro link do arquivo.

3. Segure o `Ctrl` e clique no link.

4. Faça o login no Google, caso não esteja (ou abra o link em um navegador em que o Google já está logado)

5. Na tela aberta, seleciona a opção `Criar projeto`, aceite os termos (caso precise) e clique em `Continuar`.

   - ![](CriarProjetoGoogleCloud.png)

6. Aguarde.

7. Na próxima página, clique em `Criar chave de API`.

   - ![Projeto criado](ProjetoCriado.png)

8. Aguarde.

9. Na nova tela, clique no ícone indicado para copiar a chave de API

   - ![Copiar Chave API](CopiarChaveAPI.png)

10. Volte para o Android Studio, no arquivo `google_maps_api.xml` e procure pelo seguinte trecho (geralmente no final do arquivo):

    - ```xml
      <string name="google_maps_key" templateMergeStrategy="preserve" translatable="false">YOUR_KEY_HERE</string>
      ```

11. Substitua `YOUR_KEY_HERE` pelo que acabou de copiar. No meu caso:

    - ```xml
      <string name="google_maps_key" templateMergeStrategy="preserve" translatable="false">AIzaSyASqrZlJ47Fc1715QKFRHzhD9R1mJ69OVc</string>
      ```

12. Rode a aplicação!