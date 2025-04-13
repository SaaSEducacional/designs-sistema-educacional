# Guia de Designs do Sistema Educacional SaaS

Este documento lista todos os designs SVG criados para o sistema educacional SaaS multi-tenant com Next.js e Spring Boot. Os arquivos estão organizados por categoria funcional.

## Estrutura de Arquivos

```
designs-sistema-educacional/
│
├── 1-acesso/
│   ├── login.svg                # Tela de login
│   └── cadastro.svg             # Tela de cadastro de usuário
│
├── 2-aluno/
│   ├── dashboard.svg            # Dashboard principal do aluno
│   ├── lista-cursos.svg         # Lista de cursos do aluno
│   ├── detalhe-curso.svg        # Visualização detalhada de um curso
│   ├── player-aula.svg          # Player de aula com vídeo
│   ├── simulado-quiz.svg        # Interface de simulado/quiz
│   ├── ranking.svg              # Ranking anônimo
│   ├── calendario.svg           # Calendário de aulas e eventos
│   └── perfil.svg               # Configurações de perfil
│
├── 3-professor/
│   ├── admin-dashboard.svg      # Dashboard do professor/admin
│   ├── criar-curso-info.svg     # Criação de curso - informações básicas
│   ├── criar-curso-estrutura.svg # Criação de curso - estrutura
│   ├── criar-curso-config.svg   # Criação de curso - configurações
│   ├── editar-modulo.svg        # Editor de módulo
│   ├── lesson-editor.svg        # Editor de conteúdo de aula 
│   ├── materiais-upload.svg     # Upload de materiais complementares
│   ├── criar-simulado.svg       # Criação de simulado
│   ├── quiz-question-editor.svg # Editor de questões
│   ├── agendar-aula-live.svg    # Agendamento de aula ao vivo
│   └── relatorios.svg           # Relatórios e analytics
│
├── 4-tenant-admin/
│   └── tenant-admin.svg         # Administração de tenants
│
└── design-system.md             # Documentação do design system
```

## Lista de Designs por Função

### Acesso ao Sistema
1. **Login** - Interface de autenticação com campos para email e senha
2. **Cadastro** - Formulário de registro com campos para dados pessoais e curso de interesse

### Área do Aluno
3. **Dashboard do Aluno** - Visão geral de progresso, cursos em andamento e próximas atividades
4. **Lista de Cursos** - Exibição dos cursos matriculados e disponíveis para matrícula
5. **Detalhe de Curso** - Visualização da estrutura de módulos e aulas de um curso
6. **Player de Aula** - Interface para assistir vídeos com acesso a materiais complementares
7. **Simulado/Quiz** - Interface para realização de avaliações com temporizador
8. **Ranking Anônimo** - Sistema de classificação por desempenho com codinomes
9. **Calendário** - Visualização mensal de aulas e eventos agendados
10. **Configurações de Perfil** - Interface para edição de dados pessoais

### Área do Professor/Administrador
11. **Dashboard do Professor** - Métricas e atividades recentes
12. **Criação de Curso - Informações** - Cadastro de informações básicas do curso
13. **Criação de Curso - Estrutura** - Definição de módulos e estrutura do curso
14. **Criação de Curso - Configurações** - Ajustes de visibilidade e acesso ao curso
15. **Editor de Módulo** - Interface para criar/editar módulos e gerenciar aulas
16. **Editor de Conteúdo de Aula** - Interface para upload de vídeo e conteúdo textual
17. **Upload de Materiais** - Interface para adição de materiais complementares
18. **Criação de Simulado** - Cadastro de novo simulado ou avaliação
19. **Editor de Questões** - Interface para criação e edição de questões de simulado
20. **Agendamento de Aula ao Vivo** - Interface para configurar transmissões ao vivo
21. **Relatórios e Analytics** - Visualizações gráficas de métricas e desempenho

### Administração Master (Multi-tenant)
22. **Administração de Tenants** - Gerenciamento de clientes/instituições na plataforma

## Como Usar os Designs

Os designs SVG podem ser utilizados como referência para o desenvolvimento frontend com Next.js. Eles representam a interface visual e a estrutura de interação do sistema, seguindo o design system estabelecido.

Sugestões para uso eficiente:

1. **Componentes reutilizáveis**: Identifique elementos que se repetem entre telas (botões, cards, inputs) e implemente-os como componentes React reutilizáveis.

2. **Consistência**: Mantenha a consistência visual utilizando as mesmas cores, tipografia e espaçamentos definidos no design system.

3. **Desenvolvimento por módulos**: Implemente as interfaces agrupando por funcionalidade (ex: autenticação, gestão de cursos, avaliações).

4. **Responsividade**: Adapte as interfaces para diferentes tamanhos de tela, priorizando inicialmente desktop e posteriormente adaptando para dispositivos móveis.

## Paleta de Cores

As cores principais utilizadas nos designs são:

- **Azul Principal**: `#2563eb` - Elementos principais, botões de ação primária
- **Azul Escuro**: `#1e40af` - Elementos secundários
- **Azul Muito Escuro**: `#1e293b` - Backgrounds administrativos
- **Verde**: `#10b981` - Indicadores de sucesso e conclusão
- **Amarelo/Laranja**: `#f59e0b` - Alertas e destaques
- **Vermelho**: `#ef4444` - Erros e ações destrutivas
- **Cinza Muito Claro**: `#f8fafc` - Fundo principal
- **Branco**: `#ffffff` - Cards e áreas de conteúdo

## Próximos Passos

1. Implementar os componentes base do design system em React/Next.js
2. Desenvolver as interfaces priorizando as funcionalidades essenciais (autenticação, visualização de cursos)
3. Integrar com APIs do backend Spring Boot
4. Realizar testes de usabilidade
5. Refinar e ajustar com base no feedback
