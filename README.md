# Instalação

Seguir o passo a passo do site <a href="https://k6.io/docs/getting-started/installation/">k6<a/>

## Execução 
```k6 run arquivo.js```

## Tipos de testes

### Smoke test
Avalia se com o mínimo de carga = usuários virtuais simultâneos, o sistema performa bem. Caso contrário, ajustes serão necessários nele e não compensa seguir com outros tipos de testes. Garante que o sistema funciona com carga mínima. "Teste de sanidade"
Geralmente é feito com um ou dois usuários simultâneos. 

### Load test
Verifica a performance utilizando usuários concorrentes ou várias requisições por segundo. Testa o comportamento do sistema em "condições normais". Com múltiplos acessos (usuários concorrentes) ou requisições simultâneas. "Condições normais" seria representar uma quantidade de acessos por um determinado tempo, próxima da realidade.

### Stress test e Spike testing 
Analisam os limites e picos de acesso ao sistema. Dobra, triplica a quantidade de acessos esperada para identificar quando o sistema quebra, como se recupera. Até onde aguenta? Simula um pico de acessos. Em meio a acessos constantes por tempo constante, uma alteração repentina em grande quantidade.

### Soak test
Observa o comportamento a longo prazo. Qual a resistência do sistema. Está atrelado ao tempo mais do que a quantidade de acessos. A performance resiste a horas, dias sendo testada?

## Quais tipos de testes de performance da para fazer no k6?

#### Smoke Testing -> Fumaça. 
Testa o fluxo principal. Verifica se com o mínimo de usuários virtuais simultâneos, o sistema performa bem. É o teste primário que possibilita a execução dos próximos.
#### Load Testing -> Carga. 
Testa como o sistema se comporta com usuários virtuais concorrentes ou requisições simultâneas.
#### Stress Testing -> Estresse. 
Analisa os limites do sistema. Uma quantia que quase coloca ele no máximo que aguenta. 
#### Soak/endurance Testing -> Resistência. 
Avalia a confiabilidade de performance a longo prazo (dias).
#### Spike Testing 
Testa picos altos de acesso. 

Todos os tipos de teste podem ser executádos no mesmo script com configurações diferentes. 

Como saquer qual o limite do sistema? Qual a quantidade de usuários virtuais ideal? 
Depende do sistema e o time ajuda a definir. 
Vem da análise de negócio. Requisitos de usuário, do sistema. 

