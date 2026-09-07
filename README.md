# GitHub Pages-inställning

Jag har lagt till en GitHub Actions-workflow som deployar innehållet i repo-roten till GitHub Pages när du pushar till `main` eller `master`.

Filer som lades till:

- `.github/workflows/pages.yml` — workflow för att bygga och deploya till Pages
- `.nojekyll` — förhindra Jekyll-behandling

Så här publicerar du:

1. Initiera och pusha ändringarna till ditt GitHub-repo (byt branch om du använder annan än `main`):

```bash
git add .
git commit -m "Add GitHub Pages workflow"
git push origin main
```

2. Gå till Actions-fliken på GitHub för repot och kontrollera att workflow körs.

3. När deployment är klar kommer Pages att vara publicerat. För en projekt-sida är URL:en normalt

```
https://<github-username>.github.io/<repo-namn>
```

För att jag ska kunna ge dig den exakta länken, skicka antingen GitHub-repots URL eller ditt GitHub-användarnamn och repots namn. Om du vill kan jag också hjälpa till att pusha ändringarna om du ger mig remote-access (annars kör du stegen ovan lokalt).

Notera: Om repositoryn använder skyddade grenar eller om Actions är avstängt i repo-inställningarna måste du aktivera Actions i GitHub-prouktens inställningar.
