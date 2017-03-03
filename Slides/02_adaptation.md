# S'adapter à quoi ?

<!-- .slide: class="page-title" -->



## Aux pannes

![Panne](ressources/panne.jpg)



## Aux pannes : orchestrateurs

![Orchestrateur](ressources/orchestrateur.png)



## Aux pannes : protocoles

![Raft logo](ressources/raft-logo.png)
[RAFT](https://raft.github.io/)



## Aux pannes : clustering

<iframe width="560" height="315" src="https://www.youtube.com/embed/fS9mB1Gvctw?list=PLsEeUqX8gm0N1Giw5Rsq09FmpZ5K4zsz2&start=710" frameborder="0" allowfullscreen></iframe>



## Aux pannes : testing

![Chaos Monkey](ressources/chaos-monkey.jpeg)



## A la charge

![Surcharge](ressources/surcharge.jpg)



## A la charge : autoscaling

![AWS Autoscaling](ressources/auto-scaling-on-aws-flow.png)



## A la charge : autoscaling

![ZenScaler](ressources/zenscaler.png)



<!-- .slide: class="page-demo" -->



## Parenthèse : serverless

![ServerLess](ressources/serverless.png)



## Parenthèse : serverless

```java
package example;

import com.amazonaws.services.lambda.runtime.Context;
import com.amazonaws.services.lambda.runtime.RequestHandler;

public class Hello implements RequestHandler<String, String> {
    @Override
    public String handleRequest(String input, Context context) {
    	String output = "Hello, " + input + "!";
    	return output;
    }
}
```



## Parenthèse : serverless

![Serverless framework](ressources/serverless-framework.png)




## Aux malveillances

![DDos](ressources/ddos.jpg)




## Aux malveillances

![Port scanning](ressources/port_scan.gif)




## Aux malveillances : SDN Controller

![SDN Controller](ressources/SDNController.jpg)




<!-- .slide: class="page-demo" -->



## Aux malveillances : Démo

![Archi démo](ressources/switchs-archi.png)




## Aux malveillances

![Defense4All](ressources/defense4all.png)
