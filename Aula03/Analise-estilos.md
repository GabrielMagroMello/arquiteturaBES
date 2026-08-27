# Análise de Estilos Arquiteturais

## 1. Arquitetura Monolítica

### Conceito e definição

A arquitetura monolítica organiza a aplicação como uma única unidade de software. Os principais componentes do sistema, como interface, regras de negócio e acesso aos dados, normalmente ficam reunidos dentro da mesma aplicação.

Na prática, quando o sistema é executado, seus diferentes módulos funcionam como partes de uma mesma aplicação. Uma alteração ou atualização geralmente envolve a implantação de uma nova versão do sistema como um todo.

### Casos de uso comuns

**Exemplo 1 – Sistemas administrativos:** aplicações internas de empresas podem utilizar uma estrutura monolítica para reunir cadastro de funcionários, controle de documentos e relatórios em uma única aplicação.

**Exemplo 2 – Pequenas aplicações web:** sistemas com poucos usuários e funcionalidades relativamente simples podem utilizar uma arquitetura monolítica por ser mais simples de desenvolver e implantar.

### Principais vantagens

* **Simplicidade:** possui uma estrutura relativamente simples para projetos pequenos.
* **Facilidade de desenvolvimento:** os componentes estão concentrados em uma única aplicação.
* **Facilidade de implantação:** normalmente é necessário implantar apenas uma aplicação.
* **Facilidade de testes:** pode ser mais simples testar o sistema como uma unidade.
* **Menor complexidade de infraestrutura:** não exige necessariamente diversos serviços independentes.

### Principais desvantagens

* **Escalabilidade limitada:** pode ser necessário aumentar os recursos de toda a aplicação mesmo quando apenas uma parte necessita de mais capacidade.
* **Manutenção mais difícil em sistemas grandes:** conforme o projeto cresce, o código pode se tornar complexo.
* **Implantação completa:** uma pequena alteração pode exigir a implantação de uma nova versão de toda a aplicação.
* **Maior dependência entre componentes:** alterações em uma parte podem afetar outras partes do sistema.
* **Crescimento do código:** aplicações muito grandes podem se tornar difíceis de compreender e manter.

---

## 2. Arquitetura Ponto a Ponto (Peer-to-Peer)

### Conceito e definição

A arquitetura **Ponto a Ponto (P2P)** é um modelo no qual os computadores ou dispositivos participantes podem atuar tanto como clientes quanto como servidores. Dessa forma, os participantes compartilham recursos diretamente entre si, sem depender necessariamente de um servidor central.

Na prática, um dispositivo pode solicitar um recurso a outro participante da rede e também disponibilizar seus próprios recursos para os demais. Isso permite que os participantes contribuam diretamente para o funcionamento do sistema.

### Casos de uso comuns

**Exemplo 1 – Compartilhamento de arquivos:** redes P2P podem permitir que diferentes computadores compartilhem arquivos diretamente entre si.

**Exemplo 2 – Sistemas distribuídos de comunicação:** uma rede pode utilizar o modelo P2P para permitir que os participantes troquem informações ou recursos diretamente, distribuindo o processamento e a comunicação entre os próprios dispositivos.

### Principais vantagens

* **Descentralização:** não depende necessariamente de um servidor central.
* **Compartilhamento de recursos:** os próprios participantes podem disponibilizar armazenamento, processamento ou arquivos.
* **Escalabilidade:** novos participantes podem contribuir com recursos para a rede.
* **Redução da dependência de servidores:** a ausência de um servidor central pode diminuir determinados pontos únicos de falha.
* **Distribuição da carga:** recursos e tarefas podem ser distribuídos entre diferentes participantes.

### Principais desvantagens

* **Maior complexidade de gerenciamento:** controlar uma rede formada por vários participantes pode ser mais difícil.
* **Segurança:** é necessário considerar a confiabilidade dos diferentes dispositivos conectados.
* **Disponibilidade variável:** um participante pode entrar ou sair da rede a qualquer momento.
* **Desempenho imprevisível:** a velocidade pode depender da capacidade e da conexão dos participantes.
* **Manutenção:** diagnosticar problemas pode ser mais difícil devido à natureza distribuída da arquitetura.
