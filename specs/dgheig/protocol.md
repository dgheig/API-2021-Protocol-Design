# Specification

## Protocol objectives:

> What does the protocol do?

[exp4j](https://www.baeldung.com/java-evaluate-math-expression-string) as a service
https://www.objecthunter.net/exp4j/



## Overall behavior:

- What transport protocol do we use?
  Le protocole TCP

- How does the client find the server (addresses and ports)?
  L'adresse sera connue, le port fixé à 3241

- Who speaks first?

  Le client envoie directement son expression.

- Who closes the connection and when?
  C'est le client qui ferme la connection, sauf en cas d'erreur.



## Messages:

- What is the syntax of the messages?

  L'application ne permet que de faire des calculs sans mémoire/historique.
  L'utilisateur envoie simplement son expression mathématique composée des symboles `()+-*/%^`.

  * Les valeurs décimales sont notées avec le séparateur `.`
  * le symbole `'` (guillemet simple) sera ignoré simplement ignoré. Il peut-être utilisée, par exemple, pour marquer les milliers.  

  Le serveur lui envoie ensuite la valeur numérique ou un message d'erreur

- What is the sequence of messages exchanged by the client and the server? (flow)

  Le client et le serveur s'alternent

- What happens when a message is received from the other party? (semantics)

  



## Specific elements (if useful)

- Supported operations
- Error handling
- Extensibility



## Examples: examples of some typical dialogs.
