# Projeto de Tranca Eletrônica com Arduino

## Descrição

Este projeto é uma tranca eletrônica baseada em Arduino, projetada para permitir o controle de acesso com senha. O sistema utiliza LEDs para indicar o status da senha e um piezo para alertar sobre tentativas de acesso falhas. O projeto é implementado no Tinkercad e simula uma tranca eletrônica com feedback visual e sonoro.

## Componentes

- **U1**: 1 x Arduino Uno R3
- **S1 - S7**: 7 x Botões
- **D1**: 1 x LED Verde
- **D2**: 1 x LED Vermelho
- **U2**: 1 x LCD 16 x 2
- **PIEZO1**: 1 x Piezo
- **R1**: 1 x Resistor de 1 kΩ

## Funcionalidades

- **Entrada de Senha:** O usuário pode inserir uma senha usando os botões.
- **Verificação da Senha:** A senha digitada é verificada em relação à senha cadastrada.
- **Feedback Visual:** 
  - **LED Verde (D1)**: Acende quando a senha está correta.
  - **LED Vermelho (D2)**: Acende quando a senha está incorreta.
- **Feedback Sonoro:**
  - **Piezo (PIEZO1)**: Emite um som quando a senha está incorreta.
- **Interface LCD:** Exibe mensagens e status do sistema.

## Circuito

O circuito é montado utilizando o Arduino Uno R3 como controlador central. Os botões são usados para entrada da senha, e o LED verde e vermelho fornecem feedback visual sobre a validade da senha inserida. O LCD 16 x 2 é usado para exibir informações e status, enquanto o piezo emite sons de alerta.

## Montagem

1. **Arduino Uno R3 (U1):** O controlador central do circuito.
2. **Botões (S1 - S7):** Conectados aos pinos digitais do Arduino para entrada da senha.
3. **LED Verde (D1):** Conectado a um pino digital do Arduino para indicar acesso autorizado.
4. **LED Vermelho (D2):** Conectado a um pino digital do Arduino para indicar acesso não autorizado.
5. **LCD 16 x 2 (U2):** Conectado aos pinos apropriados do Arduino para exibir mensagens.
6. **Piezo (PIEZO1):** Conectado a um pino digital do Arduino para emitir som em caso de erro.
7. **Resistor de 1 kΩ (R1):** Usado para limitar a corrente no LED.

## Código

O código-fonte para o Arduino pode ser encontrado no arquivo [codigo_arduino.ino](#). O código realiza as seguintes operações:
- Inicializa os componentes.
- Lê a entrada dos botões.
- Verifica a senha inserida.
- Controla os LEDs e o piezo com base na validade da senha.

## Instruções de Uso

1. **Configuração:** Conecte todos os componentes conforme o diagrama de circuito.
2. **Programação:** Carregue o código no Arduino usando a IDE Arduino.
3. **Operação:** 
   - Insira a senha usando os botões.
   - O LED verde acenderá se a senha estiver correta.
   - O LED vermelho e o piezo alertarão se a senha estiver incorreta.
   - O LCD exibirá mensagens sobre o status do sistema.

## Contribuições

Se você deseja contribuir para este projeto, sinta-se à vontade para enviar pull requests ou abrir problemas no [repositório GitHub](#).

## Licença

Este projeto é licenciado sob a [MIT License](LICENSE).

---

Sinta-se à vontade para modificar e adaptar este README conforme necessário para se ajustar ao seu projeto específico. Se você precisar de mais detalhes ou tiver alguma dúvida, estou aqui para ajudar!
