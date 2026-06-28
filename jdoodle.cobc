*> https://www.jdoodle.com/execute-cobol-online
*> Welcome to JDoodle!
*>
*> You can execute code here in 110+ languages. Right now you’re in the COBOL IDE.
*>
*>  1. Click the orange Execute button ▶ to execute the sample code below and see how it works.
*>  2. Want help writing or debugging code? Type a query into JDroid on the right hand side ---------------->
*>  3. Try the menu buttons on the left. Save your file, share code with friends and open saved projects.
*>
*> Want to change languages? Try the search bar up the top.

       IDENTIFICATION DIVISION.
       PROGRAM-ID. CALCULADORA.

       DATA DIVISION.
       WORKING-STORAGE SECTION.
       01 NUM-1        PIC 9(5)V9(2) VALUE 0.
       01 NUM-2        PIC 9(5)V9(2) VALUE 0.
       01 RESPOSTA     PIC 9(6)V9(2) VALUE 0.
       01 OPERACAO     PIC X VALUE SPACE.

       PROCEDURE DIVISION.
       INICIO.
           DISPLAY "DIGITE O PRIMEIRO NUMERO: ".
           ACCEPT NUM-1.

           DISPLAY "DIGITE A OPERACAO (+, -, *, /): ".
           ACCEPT OPERACAO.

           DISPLAY "DIGITE O SEGUNDO NUMERO: ".
           ACCEPT NUM-2.

           EVALUATE OPERACAO
               WHEN '+'
                   COMPUTE RESPOSTA = NUM-1 + NUM-2
                   DISPLAY "RESULTADO: " RESPOSTA
               WHEN '-'
                   COMPUTE RESPOSTA = NUM-1 - NUM-2
                   DISPLAY "RESULTADO: " RESPOSTA
               WHEN '*'
                   COMPUTE RESPOSTA = NUM-1 * NUM-2
                   DISPLAY "RESULTADO: " RESPOSTA
               WHEN '/'
                   IF NUM-2 = 0
                       DISPLAY "ERRO: DIVISAO POR ZERO!"
                   ELSE
                       COMPUTE RESPOSTA = NUM-1 / NUM-2
                       DISPLAY "RESULTADO: " RESPOSTA
                   END-IF
               WHEN OTHER
                   DISPLAY "OPERACAO INVALIDA"
           END-EVALUATE.

           STOP RUN.

