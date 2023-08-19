<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

## Descrição

Stack Laravel 10 - Docker, Apache (PHP 8.2), PostgreSQL 12 e pgAdmin4

## Instalação

**Faça o clone desse projeto:**
```bash
git clone git@github.com:WilliamJSS/stack-laravel10.git nome_do_meu_projeto
```

**Navegue para a pasta do projeto:**
```bash
cd nome_do_meu_projeto
```

**Crie o arquivo `.env` a partir do `.env.example` e adicione os valores das chaves `DB_PASSWORD` e `SGBD_PASS` com uma senha da sua preferência:**
```bash
cp .env.example .env
```
*Obs: substitua `project_name` pelo nome do seu projeto em todos os arquivos (Dica: no VSCode você pode fazer isso rapidamente na aba "Pesquisar")*

**Reinicie o repositório git:**
```bash
rm -rf .git && git init
```

## Configuração

**Suba os containers:**
```bash
docker compose up -d
```

**Acesse o terminal do container onde está o projeto:**
```bash
docker exec -it nome_do_meu_projeto_site 
```

**Execute o comando para configurar o projeto (isso irá instalar as dependências necessárias, adicionar uma chave para a aplicação e ativar o host do apache):**
```bash
npm run setup
```

## Execução

**Para rodar a aplicação, dentro do terminal do container execute o seguinte comando:**
```bash
npm run dev
```

## Links

Assim que estiver tudo configurado, você pode acessar o pgAdmin e o seu projeto pelo navegador por meio dos links abaixo:

- [Meu Projeto Laravel](http://localhost)
- [pgAdmin4](http://localhost:5050)

## Referências

- [Docker de Gêneses Lopes](https://github.com/GenesesLopes/docker)
- [Documentação do Laravel 10](https://laravel.com/docs/10.x)
- [Documentação do pgAdmin4](https://www.pgadmin.org/docs/pgadmin4/latest/index.html)
