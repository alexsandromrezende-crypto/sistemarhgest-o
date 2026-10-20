# PEGASUS — Sistema de Registro de Funcionários

## Publicar no GitHub e Vercel

1. Crie um repositório privado no GitHub.
2. Envie os arquivos `index.html` e `vercel.json` na raiz.
3. Na Vercel, acesse **Add New → Project**, importe o repositório e selecione **Other** como Framework Preset, sem build command.
4. Faça o deploy. A Vercel serve `index.html` e fornece HTTPS para solicitar permissão da câmera.
5. Clique em **Abrir câmera** e autorize o navegador. Ou selecione uma imagem do dispositivo.

## Mantido
Todos os campos originais; validações; dependentes; matrícula automática; cadastros; PDF; CSV; arquivar, restaurar e remover.

## Novidades
Câmera com captura e troca de câmera; arquivo do computador; otimização da foto sem distorção; prévia e remoção; visual responsivo; indicadores e persistência por `localStorage`.

## Limites de segurança
**Esta é uma versão estática demonstrativa.** Os dados ficam no `localStorage` do navegador e NÃO são sincronizados entre equipamentos ou usuários. Eles podem ser perdidos se os dados do site forem apagados ou o navegador estiver em modo privado. Não há autenticação, banco de dados, backup nem controle de acesso. Como o cadastro contém CPF, RG, contato e remuneração, **não use esta versão em produção para dados pessoais reais**. Implemente banco de dados com autenticação e regras de autorização (por exemplo, Supabase ou Firebase) em implantação institucional. Não publique planilhas, fotos ou cadastros no repositório. Bibliotecas PDF são carregadas de CDN, exigindo internet.

Referências técnicas: https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices/getUserMedia e https://vercel.com/docs/deployments/git
