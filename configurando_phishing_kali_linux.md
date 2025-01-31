
# Configurando o Phishing no Kali Linux

No Kali Linux, a configuração de phishing envolve o uso de ferramentas específicas para simular ataques de phishing, como o *Social Engineering Toolkit* (SET), que é uma das mais populares. Lembre-se de que a realização de ataques de phishing sem permissão é ilegal e antiética. Sempre use essas ferramentas em ambientes controlados e com permissão explícita.

## Passos para configurar o phishing no Kali Linux

### 1. Atualize o Kali Linux
Antes de começar, sempre é bom garantir que o sistema esteja atualizado. No terminal, execute:

```bash
sudo apt update && sudo apt upgrade -y
```

### 2. Instalar o Social Engineering Toolkit (SET)
O SET geralmente já está instalado no Kali Linux, mas caso não esteja, você pode instalar com o seguinte comando:

```bash
sudo apt install set
```

### 3. Iniciar o SET
Após a instalação, inicie o SET com o seguinte comando:

```bash
sudo setoolkit
```

### 4. Escolher o ataque de phishing
O SET oferece várias opções de ataques baseados em engenharia social. Para configurar um ataque de phishing, siga os seguintes passos:

- **Selecione a opção 1** para "Social-Engineering Attacks"
- **Selecione a opção 3** para "Phishing Attack Vectors"
- Em seguida, você verá várias opções para diferentes tipos de phishing. Selecione a opção que deseja, como "Site Cloner" (que clona um site legítimo e captura credenciais quando o usuário interage com o site falso).

### 5. Configurar o phishing
Quando você escolhe, por exemplo, "Site Cloner", será solicitado a informar o site legítimo que deseja clonar (por exemplo, "https://www.google.com").

### 6. Configurar o servidor web
Após clonar o site, o SET configurará um servidor web no Kali Linux para hospedar a página clonada e aguardar as interações. O SET geralmente configura automaticamente a porta para o servidor.

### 7. Executar o ataque
Quando o atacante interage com o site falso, você pode capturar credenciais e outros dados inseridos pelo usuário.

### 8. Monitorar os resultados
O SET irá gerar logs com os dados coletados, como nomes de usuário e senhas, que serão armazenados em um arquivo.

## Atenção
Novamente, sempre use essas ferramentas em um ambiente de teste ou com permissão explícita. O uso inadequado pode resultar em sérias consequências legais.
