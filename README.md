# LimpaCache
Algoritmo que limpa arquivos temporários.

O código C# realiza a limpeza de arquivos temporários em várias localizações do sistema. Ele segue os seguintes passos:

Obtém Diretórios Temporários:

Identifica os diretórios de arquivos temporários comuns, incluindo:
O diretório temporário do usuário (%TEMP%).
O diretório temporário especificado pela variável de ambiente %TMP%.
O diretório Temp no diretório do sistema Windows (%SystemRoot%\Temp).
Limpeza dos Diretórios:

Para cada diretório identificado:
Arquivos: Deleta todos os arquivos encontrados no diretório.
Diretórios: Deleta todos os subdiretórios e seu conteúdo.
Tratamento de Exceções:

Se ocorrer um erro ao deletar arquivos ou diretórios, ele captura e exibe a mensagem de erro correspondente.
Execução e Relatórios:

Imprime mensagens informativas sobre quais arquivos e diretórios foram deletados e quaisquer problemas encontrados durante o processo.
Funções Principais:
ClearTemporaryFiles(): Função que realiza a limpeza de arquivos temporários em vários diretórios.
Path.GetTempPath(): Obtém o caminho do diretório temporário do usuário.
Environment.GetEnvironmentVariable("TEMP") e Environment.GetEnvironmentVariable("TMP"): Obtêm os caminhos dos diretórios temporários especificados pelas variáveis de ambiente.
Directory.Delete() e File.Delete(): Usados para remover arquivos e diretórios.
Nota:
O código pode precisar de permissões elevadas para acessar e deletar certos arquivos e diretórios.
Deve ser usado com cuidado para evitar a exclusão acidental de arquivos importantes.
Esse resumo oferece uma visão geral das funcionalidades e operações principais do script de limpeza de cache.
