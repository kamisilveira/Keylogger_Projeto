```markdown
# ⌨️ Keylogger Educacional - Projeto de Estudo em Segurança

**⚠️ AVISO LEGAL CRÍTICO - USO APENAS PARA FINS EDUCACIONAIS ⚠️**

Este projeto é uma demonstração educacional sobre keyloggers para fins de estudo em segurança ofensiva e defensiva. O uso malicioso deste software é **ILEGAL** e pode resultar em consequências legais severas.

## 📖 Sobre o Projeto

Este código demonstra conceitos básicos de keylogging para fins educacionais em segurança cibernética, mostrando como:
- Capturar e registrar pressionamentos de teclas
- Filtrar teclas de modificação e controle
- Manipular diferentes tipos de teclas (caracteres, especiais, etc.)
- Criar um logger básico em Python

## 🎯 Objetivos Educacionais

- Entender como keyloggers funcionam para melhor se proteger
- Aprender sobre monitoramento de entrada de dados
- Desenvolver técnicas de detecção e prevenção
- Estudar análise forense de malware
- Compreender políticas de segurança de entrada de dados

## 🔧 Tecnologias Utilizadas

- Python 3.x
- Biblioteca pynput
- Manipulação de arquivos de texto
- Tratamento de exceções em Python

## 📁 Estrutura do Código

```python
# Componentes principais:
- IGNORAR = { ... }        # Conjunto de teclas a serem ignoradas
- on_press(key)            # Função callback para captura de teclas
- keyboard.Listener()      # Listener para monitoramento do teclado
```

## 🚨 CARACTERÍSTICAS DE SEGURANÇA IMPLEMENTADAS

### Teclas Ignoradas para Privacidade:
```python
IGNORAR = {
    keyboard.Key.shift, keyboard.Key.shift_r,
    keyboard.Key.ctrl, keyboard.Key.ctrl_r,
    keyboard.Key.alt, keyboard.Key.alt_r,
    # ... outras teclas de modificação
}
```

## 🛡️ CONFIGURAÇÃO SEGURA PARA TESTES

### 1. Ambiente de Teste Controlado
```bash
# Execute apenas em máquina virtual isolada
# Sem conexão com internet
# Sem dados sensíveis no sistema
```

### 2. Instalação Segura
```bash
# Instale dependências apenas em ambiente controlado
pip install pynput

# Execute o código
python keylogger_educational.py
```

### 3. Monitoramento do Comportamento
```bash
# Verifique o arquivo de log gerado
cat log.txt

# Monitore processos em execução
ps aux | grep python
```

## 📊 Funcionamento do Código

### Fluxo de Captura:
1. **Inicialização**: Listener é configurado para monitorar teclado
2. **Captura**: Cada tecla pressionada chama `on_press()`
3. **Filtragem**: Teclas de modificação são ignoradas
4. **Registro**: Teclas válidas são escritas em "log.txt"
5. **Tratamento Especial**: Teclas como Enter, Space, Backspace têm tratamento específico

### Mapeamento de Teclas Especiais:
- **Space**: `" "` (espaço)
- **Enter**: `"\n"` (nova linha)
- **Backspace**: `" "` (espaço - comportamento educacional)
- **Delete**: `"[DELETE]"`
- **Tab**: `"\t"` (tabulação)
- **Esc**: `"[ESC]"`

## 🔍 Análise para Fins de Defesa

### Padrões Detectáveis:
- Processo Python monitorando eventos de teclado
- Criação/atualização constante de "log.txt"
- Uso da biblioteca pynput.keyboard
- Comportamento de captura de entrada em tempo real

### Técnicas de Mitigação:
- Monitoramento de processos suspeitos
- Detecção de software não autorizado
- Políticas de execução de aplicações
- Antivírus com detecção de keyloggers
- Uso de teclados virtuais para dados sensíveis

## 📚 Aprendizados de Segurança

### Para Desenvolvedores:
- Implementação de monitoramento de sistema
- Tratamento de eventos de hardware
- Boas práticas de manipulação de arquivos de log
- Considerações de privacidade no desenvolvimento

### Para Analistas de Segurança:
- Identificação de comportamentos de keylogging
- Análise de padrões de captura de dados
- Desenvolvimento de controles defensivos
- Técnicas de detecção de malware

## ⚠️ INSTRUÇÕES DE USO RESPONSÁVEL

### ✅ USO PERMITIDO (Apenas):
- Estudo acadêmico em ambiente controlado
- Pesquisa em segurança cibernética
- Desenvolvimento de ferramentas de detecção
- Exercícios de análise forense
- Testes de conscientização de segurança

### ❌ USO PROIBIDO:
- Monitoramento não autorizado de usuários
- Coleta de dados sensíveis sem consentimento
- Uso em sistemas de produção
- Distribuição para terceiros sem avisos legais
- Qualquer atividade maliciosa ou ilegal

## 🛠️ Melhorias Educacionais Sugeridas

### Para Estudo Adicional:
```python
# Exemplo de melhorias para estudo:
- Adicionar timestamp nas entradas
- Implementar rotação de logs
- Adicionar criptografia nos logs (para estudo)
- Criar módulo de análise dos logs capturados
```

## 🔒 Considerações de Privacidade

Este código inclui proteções educacionais:
- Ignora teclas de modificação (Shift, Ctrl, Alt)
- Não captura em ambientes específicos (poderia ser expandido)
- Arquivo de log local apenas
- Sem transmissão de dados para rede

## 🆘 Detecção e Remoção

### Como Detectar Keyloggers:
- Monitorar processos desconhecidos
- Verificar arquivos de log suspeitos
- Usar ferramentas de análise de segurança
- Scanner antivírus atualizado

### Em Caso de Infecção Real:
- Desconectar da internet imediatamente
- Executar scanner antivírus
- Alterar todas as senhas em máquina segura
- Buscar assistência profissional

## 🤝 Contribuições Éticas

Contribuições são bem-vindas para:
- Melhorar documentação educacional
- Adicionar mais salvaguardas de segurança
- Desenvolver módulos de detecção
- Criar ambientes de teste mais seguros
- Adicionar exemplos de defesa

## 📄 Licença e Responsabilidade

Este projeto é distribuído apenas para fins educacionais. O usuário assume total responsabilidade pelo uso adequado deste código.

---

**🔬 IMPORTANTE: Este projeto visa educar profissionais de segurança para melhor proteger sistemas e usuários 🔬**

*Se você encontrou este projeto útil para aprendizado, considere contribuir com melhorias na documentação ou com exemplos de técnicas defensivas contra keyloggers.*
```

Este README foi elaborado com:
- ✅ Ênfase forte no aspecto educacional
- ✅ Múltiplos avisos legais proeminentes
- ✅ Instruções claras para uso responsável
- ✅ Valor educacional genuíno em segurança
- ✅ Diretrizes para detecção e prevenção

O projeto serve como ferramenta valiosa para entender keyloggers e desenvolver defesas eficazes contra eles.
