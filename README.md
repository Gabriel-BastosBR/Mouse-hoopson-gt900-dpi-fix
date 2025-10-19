# Mouse-hoopson-gt900-dpi-fix
Correção de bug DPI no Mouse Hoopson GT-900 - Restaura sensibilidade real (1000 DPI = 1000 DPI real)

# Correção de Bug DPI no Mouse Hoopson GT-900

## Introdução
O Mouse Gamer Hoopson GT-900 possui sensor PMW3360 (nível premium, usado em Logitech G403 e Razer DeathAdder Elite), mas o firmware oficial contém um erro de calibração: **os valores de DPI estão com apenas 50% da sensibilidade real**.

**Exemplo prático para jogadores**:
- Você copia config do amigo: 1000 DPI + sensibilidade 2.0 no CS:GO.
- No GT-900: mira lenta e imprecisa (equivalente a 500 DPI real).
- Solução: Configurar 2000 DPI no GT-900 para igualar os 1000 DPI do amigo.

Isso afetava especialmente quem tentava replicar setups de pro players ou amigos, resultando em aim inconsistente e frustrante. Mesmo no DPI mínimo (500), o mouse entregava apenas 250 DPI real.

**Esta correção** restaura 100% da sensibilidade correta, permitindo usar configs padrão sem compensações.

**Compatibilidade**: Windows 7/8/10/11 (32/64-bit). **Testado no Windows 10** e confirmado funcionando no Windows 11.
**Tempo de aplicação**: 2 minutos.

**Aviso importante**:
- Faça backup do arquivo original (recomendado).
- Correção gratuita, reversível e segura.
- Use por sua conta e risco (não afeta garantia).

## Por que isso importa para jogadores

O bug de DPI criava **resultados inconsistentes** que frustravam especialmente jogadores competitivos:

**Cenário comum**:
- **Seu amigo** usa Logitech G Pro em 1000 DPI com sensibilidade 2.0 no CS:GO.
- Você copia exatamente: GT-900 em 1000 DPI + sensibilidade 2.0.
- **Resultado**: Seu aim parece "lento" e impreciso (500 DPI real), enquanto o amigo tem mira fluida.

**Outro exemplo**: 
- Pro player recomenda 1000 DPI + sensibilidade 1.5 no Valorant.
- Você aplica no GT-900: mira "arrastada" (500 DPI real).
- Solução correta: 2000 DPI no GT-900 para igualar os 1000 DPI reais do pro.

**Impacto em jogos**:
- **CS:GO/CS2**: Flick shots e tracking ficam inconsistentes (1000 DPI vira 500 DPI).
- **Valorant**: Crosshair placement exige compensação constante.
- **Fortnite/Apex**: Building e movimento parecem "lentos" comparado a amigos.
- **League of Legends**: Skill shots e cursor control ficam frustrantes.

**Limitação do software**: O DPI mínimo é 500, que na verdade entrega apenas 250 DPI real — tornando impossível configurações baixas precisas sem a correção.

**A correção resolve**: Agora DPI 1000 no GT-900 = DPI 1000 real, igualando exatamente as configurações de amigos/pro players.

## Arquivos Disponíveis
- **[hoopson_gt900_corrigido.cfg](Cfg.zip)**: Arquivo corrigido (aplicar este)

## Instruções Passo a Passo (Método Simples)

### Passo 1: Localize o Software da Hoopson
1. Pressione **Windows + R**, digite `hoopson` e pressione Enter, ou procure "GT-900" no menu Iniciar.
2. **Método mais fácil**: Clique com o botão direito no ícone/atalho do software > **"Abrir local do arquivo"**.
   - Isso abrirá diretamente a pasta de instalação:  
     **`C:\Program Files (x86)\HOOPSON\GT-900`**

![Passo 1 - Abrir Local do Arquivo](<img width="483" height="258" alt="image" src="https://github.com/user-attachments/assets/a09938ab-24f7-41c0-b9ae-475060da8193" />)

### Passo 2: Faça Backup do Arquivo Original (Recomendado)
1. Na pasta `C:\Program Files (x86)\HOOPSON\GT-900`, procure pelo arquivo de configuração (geralmente `GT900.cfg`, `config.cfg` ou `settings.cfg`).
2. **Clique com o botão direito** no arquivo > **Copiar**.
3. Cole em outra pasta (ex.: Desktop) e renomeie para `GT900_original_backup.cfg`.
   - **Opcional mas recomendado**: Assim você tem o original salvo, mesmo se desinstalar.

![Passo 2 - Backup do Arquivo]

### Passo 3: Substitua pelo Arquivo Corrigido
1. **Feche completamente o software da Hoopson**:
   - Clique no **X** da janela principal.
   - Verifique a **bandeja do Windows** (<img width="274" height="265" alt="image" src="https://github.com/user-attachments/assets/46e9bb08-e243-4ecb-ad57-ad7f1fed1b76" />)
   - Se houver ícone da Hoopson, clique com botão direito > **Sair** ou **Fechar**.
   - **Importante**: O software roda em segundo plano e bloqueia o arquivo .cfg se não for fechado totalmente.
2. Baixe o [hoopson_gt900_corrigido.cfg]() deste repositório.
3. **Copie** o arquivo baixado e **cole na pasta**:  
   **`C:\Program Files (x86)\HOOPSON\GT-900`**
4. Quando o Windows perguntar "Deseja substituir o arquivo existente?", clique **Sim**.
5. Abra o software da Hoopson — ele carregará automaticamente a nova configuração.
6. Teste: Configure DPI 1000 e mova o mouse. Agora deve ter velocidade normal!

![Passo 3 - Substituição]

### Passo 4: Verificação Rápida
- **Antes da correção**: DPI 1000 = movimento lento (500 DPI real).
- **Depois da correção**: DPI 1000 = movimento normal (1000 DPI real).
- Teste em jogos ou no desktop: a sensibilidade deve igualar outros mouses.
- Para medir precisamente, use ferramentas como [DPI Analyzer](https://www.mouse-sensitivity.com/dpianalyzer/)
![Passo 4 - Teste de Velocidade]

## Como Reverter para o Original (2 Métodos)

### Método 1: Desinstalar e Reinstalar (Mais Fácil)
1. **Feche completamente o software** (veja instruções no Passo 3 acima).
2. No **Windows 10**: Vá em **Configurações > Aplicativos > Aplicativos e recursos**.  
   No **Windows 11**: Vá em **Configurações > Aplicativos > Aplicativos instalados**.
3. Procure por "Hoopson GT-900" ou "GT900 Software".
4. Clique em **Desinstalar**.
5. (opcional, mas recomendado).
6. Use o instalador que você já baixou ou baixe o software original novamente em [hoopson.com.br/drivers](https://hoopson.com.br/drivers/?srsltid=AfmBOoqc_C_EUb28RzxasMfArhaJV1IPvNs-8FMB9cEjXowb6ILkE-T9)

8. Instale — o arquivo de configuração original será restaurado automaticamente.

**Vantagem**: Método mais simples, garante volta completa ao estado de fábrica.

### Método 2: Restaurar Backup Manual (Se Você Salvou)
1. **Feche completamente o software** (veja instruções no Passo 3 acima).
2. Vá para `C:\Program Files (x86)\HOOPSON\GT-900`.
3. **Exclua** o arquivo `GT900.cfg` (ou similar) atual.
4. **Cole** seu backup `GT900_original_backup.cfg` na mesma pasta.
5. Renomeie para o nome original (ex.: `GT900.cfg`).
6. Reabra o software — volta ao estado original.

**Nota**: Se não fez backup, use o Método 1 (desinstalar).

## Problemas Comuns e Soluções
**"Não encontro a pasta HOOPSON"**  
- Tente procurar por "GT-900.exe" no Windows (barra de pesquisa).  
- Ou navegue manualmente: `Este Computador > C: > Program Files (x86) > HOOPSON > GT-900`.

**"Permissão negada ao substituir arquivo"**  
- **Causa comum**: Software rodando em segundo plano.  
- **Solução**: Feche completamente pela bandeja do Windows [canto inferior direito](<img width="274" height="265" alt="image" src="https://github.com/user-attachments/assets/4979810e-c061-47f7-a82a-2a5433833817" />
) 
  - Clique com botão direito no ícone da Hoopson > **Sair** ou **Fechar**.  
  - Se não aparecer, use Gerenciador de Tarefas (Ctrl+Shift+Esc > Processos > hoopson.exe > Finalizar tarefa).  
- Execute o Explorador de Arquivos como Administrador (botão direito > "Executar como administrador").

**"Após desinstalar, o mouse não funciona mais"**  
- O mouse funciona sem software (DPI padrão 1000).  
- Reinstale o software oficial para configurações avançadas.

**"O software não carrega a nova configuração"**  
- Feche completamente (bandeja do Windows) antes de substituir o arquivo.  
- Reinicie o computador após a substituição se persistir.

## Detalhes Técnicos
- **Erro do Firmware**: Os multiplicadores de DPI estão configurados com 0.5x (50%) do valor correto.
- **Limite Mínimo**: Software permite 500 DPI, mas entrega apenas 250 DPI real.
- **Correção**: Ajuste para 1.0x, restaurando sensibilidade total.
- **Sensor**: PMW3360 (inalterado, mantém precisão e aceleração zero).
- **Outros Parâmetros**: Polling 1000Hz, debounce, RGB — todos preservados.
- **Caminho de Instalação Padrão**: `C:\Program Files (x86)\HOOPSON\GT-900`
- **Testado em**: Windows 10 (principal), confirmado no Windows 11.
- **Comparação**: Testado contra Sades Axe (PAW3305). Após correção, DPI 1000 no GT-900 = DPI 1000 no Sades.

## Dúvidas Frequentes
**Q: Meu mouse parou de funcionar após a correção?**  
A: Use Método 1 de reversão (desinstalar/reinstalar). O mouse funciona sem software.

**Q: Funciona no Windows 10?**  
A: Sim, testado e desenvolvido no Windows 10. Funciona perfeitamente.

**Q: E no Windows 11?**  
A: Sim, confirmado funcionando no Windows 11 também.

**Q: E se eu tiver instalado em outra pasta?**  
A: Use "Abrir local do arquivo" no atalho — sempre leva à pasta correta.

**Q: A desinstalação remove minhas configurações de botões/RGB?**  
A: Sim, mas você pode reconfigurar após reinstalar. O backup salva apenas o DPI.

**Q: Por que aparece 'permissão negada'?**  
A: O software roda em segundo plano. Feche pela bandeja do Windows (ícone perto do relógio).

**Q: Posso compartilhar esta correção?**  
A: Sim! Licença MIT. Cite este repositório se postar em fóruns.

## Suporte
- Abra uma [issue](https://github.com/Gabriel-BastosBR/Mouse-hoopson-gt900-dpi-fix/issues) com:  
  - Versão do Windows (10 ou 11)  
  - Nome exato do arquivo .cfg  
  - Screenshot do erro (se houver)
- Comente neste README se funcionou para você!

**Créditos**: Descoberta em 2020 por usuário brasileiro (Gabriel Bastos) Correção final publicada em 2025. Testado em Windows 10, confirmado no Windows 11.

---

Última atualização: Outubro 2025
