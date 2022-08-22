# Instalação

Seguir o passo a passo do site <a href="https://k6.io/docs/getting-started/installation/">k6<a/>

## Execução 
```
k6 run arquivo.js
```

## Tipos de testes

### Smoke test
Avalia se com o mínimo de carga = usuários virtuais simultâneos, o sistema performa bem. Caso contrário, ajustes serão necessários nele e não compensa seguir com outros tipos de testes. 

### Load test
Verifica a performance utilizando usuários concorrentes ou várias requisições por segundo. 

### Stress test e Spike testing 
Analisam os limites e picos de acesso ao sistema.

### Soak test
Observa o comportamento a longo prazo. Qual a resistência do sistema. 
