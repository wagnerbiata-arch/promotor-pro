PROMOTOR PRO — PACOTE PWA PARA IPAD
===================================

O QUE ESTA VERSAO FAZ
- Cadastro, edição, busca e exclusão de clientes.
- Importação de carteira por CSV (exportado do Excel/Numbers).
- Roteiro filtrado por cidade, em ordem de bairro e nome.
- Registro de início/fim, objetivo, relato e encaminhamentos de visitas.
- Anexar fotos às visitas (as imagens são reduzidas para economizar espaço).
- Relatórios por status e cidade.
- Exportação CSV de clientes e visitas, compatível com Excel/Numbers.
- Backup completo e restauração em JSON.
- Armazenamento local no navegador (IndexedDB), com cache offline.
- Nenhum uso de GPS, localização ou geolocalização.

IMPORTANTE SOBRE INSTALACAO NO IPAD
Este ZIP contém o aplicativo web e seus arquivos. Para instalar como ícone na tela inicial e habilitar o cache offline do Safari, o pacote precisa ser publicado uma vez em um endereço HTTPS. O Service Worker/PWA não funciona ao abrir o index.html diretamente pelo app Arquivos (file://).

PASSOS PARA PUBLICAR
1. Extraia a pasta PromotorPro-PWA.
2. Publique o CONTEUDO da pasta em um serviço de hospedagem estática HTTPS (por exemplo, GitHub Pages, Cloudflare Pages ou Netlify).
3. Abra o endereço HTTPS no Safari do iPad.
4. Toque em Compartilhar > Adicionar à Tela de Início > Adicionar.
5. Abra pelo ícone criado. Depois do primeiro carregamento completo, o app poderá abrir offline.

DADOS E BACKUP
- Os dados ficam no armazenamento local do Safari neste iPad e não são enviados a um servidor pelo código deste aplicativo.
- Limpar os dados do site/navegador pode apagar a carteira e o histórico. Use Relatórios > Fazer backup completo (JSON) regularmente e guarde o arquivo no app Arquivos/iCloud Drive.
- A restauração substitui os dados atuais; faça backup antes.
- A exportação Excel é CSV separado por ponto e vírgula, que abre no Excel e Numbers. O app não gera XLSX nativo nesta versão.
- Importação: Excel/Numbers > Exportar/Salvar como CSV UTF-8. Coluna obrigatória: Nome ou Empresa. Colunas reconhecidas: CNPJ, Responsável, Telefone, Cidade, Bairro, Endereço, CEP, Marcas e Observações. Clientes com CNPJ repetido são ignorados.

LIMITACOES
- A publicação HTTPS ainda precisa ser feita numa conta de hospedagem escolhida pelo usuário; este pacote não cria conta nem publica automaticamente.
- Fotos e dados dependem do armazenamento disponível no iPad.
- O Safari pode suspender/limitar armazenamento se o dispositivo estiver com pouco espaço; mantenha backups.
- Validação de visita é administrativa: status Realizada após preenchimento do relato e registro de horário. Não comprova presença física.
