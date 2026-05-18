# Why is US Healthcare So Expensive?

A structured analysis of the economic, regulatory, and systemic factors that make healthcare in the United States extraordinarily expensive compared to other developed nations.

## Overview

A reasoning process from first principles: starting from basic economic assumptions (competition should lower prices) and discovering why those assumptions break down in the US healthcare system.

## Key Question

If competition normally reduces prices, **why doesn't it work in US healthcare?**

## Structure

- **[Main Analysis Tree](main-tree.md)** - Hierarchical breakdown of causes and consequences
- **[facts/](facts/)** - Detailed explanations of individual factors
- **[resources/](resources/)** - Supporting data, examples, and potential solutions

## Quick Summary

The US healthcare system is trapped in a **Nash equilibrium** where:
- Hospitals have local monopoly power
- Insurers profit from high costs (not low ones)
- Patients cannot choose providers during emergencies
- Massive barriers prevent new competitors from entering
- Legal and regulatory structures reinforce this equilibrium

Result: Costs 2-3× higher than comparable nations, without better outcomes.

## Navigation

Start with the [Main Analysis Tree](main-tree.md) to see the complete causal structure, then dive into specific topics in the `facts/` directory.

---

*A living document — explores healthcare economics through systematic reasoning. Spanish version below.*

## English version
In this piece I want to find out, from the point of view of someone who has no idea about the healthcare system in the US, what is the fundamental reason why healthcare is so expensive there. At the end I'll lay out the specific things that, if changed, could let the system work even better than in Europe.

Lots of people say "Capitalism doesn't work — do you want healthcare to be so expensive like in the US? Sure, you have lots of toys, but no healthcare." Hear me out: capitalism is not the problem here. Not even close. The problem is the incentive structure created by the regulations.

Let's think this through. Imagine you have complete freedom to create hospitals and insurance companies that work with those hospitals, and in the US you can get a lot more revenue for the same work, in the same hospital, with the same machines. Where are you going to build your hospital? In the US you'll earn a lot more money, so the decision is clear. Now the question is: why aren't lots and lots of hospitals being created in the US to take advantage of this opportunity? Something is blocking this process. That's what we have to figure out. Free-market capitalism would cause hospitals to compete and drive prices down — but that's not what we see.

*(English version is currently a stub — the full reasoning lives in the Spanish version below and in the [Main Analysis Tree](main-tree.md).)*

## Spanish version
En este video, desde el punto de vista de alguien que no tiene ni idea, vamos a intentar entender la razón fundamental por la que la sanidad es tan cara en los estados unidos. Es algo que siempre he querido entender bien pero no me ha llegado a quedar claro exactamente por qué es así.

Como dato, una apendicitis cuesta entre 25 y 60k vs 3-8k en México, unas cataratas 5k vs 1k en México, la UCI cuesta unos 10k al día vs 1k en México.

La primera respuesta que dan es que los precios son altos por la falta de regulación, pero si fuese cierto que hay poca regulación, la competencia debería hacer que los precios bajen. Hay un incentivo muy fuerte para crear hospitales, con costes más o menos similares a los del resto del mundo, y cobrar precios mucho más altos sin perder clientes. Si los precios siguen siendo altos, es porque debe haber algo que impide este proceso.

El primer punto es sobre la competencia. En situaciones de emergencia, como un infarto, no tienes tiempo para comparar precios entre hospitales, y eso elimina la presión competitiva. Sin embargo, las aseguradoras sí pueden negociar precios fijos para cada procedimiento, eliminando esta carga de los pacientes. Las aseguradoras tienen incentivos para negociar precios bajos y así poder ofrecer primas más competitivas a sus clientes. Hay quien dice que cobran un porcentaje sobre el coste de los procedimientos y están incentivadas a que los costes sean altos, pero yo mañana creo una aseguradora que consiga costes hospitalarios bajos, puedo llevarme a todos los clientes y hacer que las aseguradoras tradicionales quiebren, así que el incentivo de competir está ahí, y no creo que esta cuestión sobre la competencia sea un motivo relevante. 

Para organizar el análisis, podemos simular mentalmente que vamos a crear un hospital con precios normales, vamos a tener muchos clientes y vamos a ganar mucho dinero. ALGO nos va a parar.

Resulta que cuando queramos abrir el hospital y negociar con las aseguradoras, no van a querer trabajar con nosotros, porque los hospitales tradicionales las están chantajeando y dicen: "Si incluyes a este hospital barato en tu red, nosotros nos vamos." Y la aseguradora se queda sin la gran mayoría de hospitales, y deja de poder garantizar a sus clientes el acceso a los hospitales principales, que son necesarios en caso de emergencias.

Lo primero, no debería ser legal hacer eso. Al menos no en este sector. Si el dumping es ilegal, la colusión para fijar precios, la competencia desleal, y la manipulación del mercado son ilegales. Esto debería ser ilegal también. En general no me gusta añadir restricciones y regulaciones, pero en un sector que está ya tan regulado, esto no me parece mal. Garantiza la competencia.

El problema es que es muy difícil probar que está ocurriendo, y no han acabado los contratos por otro motivo. Es complicado porque si decidimos crear nuestra propia aseguradora, seguimos teniendo el mismo problema, la mayoría de hospitales no querrán trabajar con nosotros.

Aquí una solución sería el control de precios, como hacen la mayoría de países europeos, por ejemplo Holanda es un buen sistema, pero creo que un buen entorno de competencia libre puede llegar a reducir los precios todavía más, con mejor calidad. El ánimo de lucro incentiva mucho más la innovación y la eficiencia, que por ejemplo los sistemas de hospitales privados sin ánimo de lucro o cooperativos. Permite que unas pocas personas arriesguen mucho capital para crear algo nuevo y mejor, lo cual no ocurre con facilidad en sistemas cooperativos.

Vamos a pensar problemas más sencillos primero, problemas como las cataratas, que no son emergencias y sí nos permiten elegir hospitales o centros más baratos, pero aun así son 5 veces más caras que en mexico. Qué me impide a mi abrir una clínica especializada en cataratas. Lo he estado investigando y resulta que el Coste de responsabilidad civil son entre 30 y 80k al año, porque el sistema legal americano suele aplicar castigos económicos muy altos (daño punitivo), a diferencia de Europa donde suelen ser compensaciones más razonables. Aun así, por qué no se puede pre-negociar por contrato que si hay algún tipo de negligencia, las compensaciones serán estas y el juicio se realizará con este árbitro en vez de un tribunal normal?

Pues resulta que "Las “waivers” (renuncias) son ilegales en sanidad". Si se firmara un contrato así, el juez lo invalidaría.

Esta es el segundo problema fundamental. Si se acuerda por contrato y el contrato es realmente fácil de comprender y está en unos rangos razonables, no debería haber problema. El resto del mundo lo hace así y no pasa nada.

El tercer problema regulatorio que habría que modificar en muchos estados es el Certificate of Need (CON). Resulta que para crear un centro de cirugía ambulatoria, que es un lugar donde se opere a la gente sin necesidad de que duerman en el hospital, el estado tiene que aportar el certificado de necesidad, donde pregunta a los hospitales existentes si “hace falta” tu centro, y si los hospitales niegan la necesidad, te niegan el permiso.

Aunque el centro no haga falta, debería permitirse su creación siempre que cumpla con los requisitos de calidad. El estado no es quien para juzgar si es necesario o no. Está bien que el estado los cree cuando lo vea necesario, pero NO al revés. No hay ningún motivo por el que el estado deba impedir la creación de un centro de cirugía ambulatoria, porque no lo considere necesario, eso es competencia desleal.

Otro problema es Medicare. Medicare es el sistema de seguro médico del gobierno para mayores de 65 años, y cubre a más de 65 millones de personas. Al ser un pagador tan grande, Medicare debería tener un poder de negociación enorme con los hospitales, similar al que tienen los gobiernos europeos. Sin embargo, hay una ley federal (creada por lobbying de la industria farmacéutica y hospitalaria) que **prohíbe a Medicare negociar precios de forma agresiva** en muchos casos. Por ejemplo, hasta 2022 Medicare tenía prohibido por ley negociar precios de medicamentos. Esto es absurdo: tienes el comprador más grande del país y le prohibes usar su poder de negociación. Es como si Amazon no pudiera pedir descuentos por volumen. Esta restricción legal es otra barrera artificial que mantiene los precios altos

Se me ocurre que un camino que podría servir para competir con los hospitales tradicionales sin necesidad de prohibir el chantaje que están llevando a cabo en la actualidad, sería inicialmente especializarse en procedimientos no urgentes y de bajo riesgo, ir añadiendo poco a poco procedimientos más complejos y de mayor riesgo, y llegado el punto en el que la mayor parte de hospitales o centros puedan adaptarse facilmente para tratar urgencias, la presión sería demasiado fuerte y las aseguradoras acabarían negociando con estos nuevos hospitales, eliminando el oligopolio actual.

Otra razón por la que los costes son tan altos es el coste laboral. Son 2-4 veces más altos que en Europa. Un enfermero en España cobra unos 25.000€ al año, en Estados Unidos 75-90.000$. Un médico en Europa cobra 70-150k, en Estados Unidos 200-600k. Como los salarios son 50-60% del coste de un hospital, esto multiplica por 2-3 el coste total.

La pregunta obvia es: ¿por qué no hay más inmigración? Si un enfermero filipino o español puede ganar el triple viniendo a Estados Unidos, debería haber una avalancha de trabajadores sanitarios emigrando, lo cual aumentaría la oferta y reduciría los salarios a niveles razonables.

Resulta que hay barreras de inmigración extremadamente restrictivas. Las visas H-1B para trabajadores cualificados tienen un límite de unas 85.000 al año para TODAS las industrias (tecnología, sanidad, finanzas, etc.), y se asignan por lotería. Además, cada estado tiene sus propios requisitos de licencia médica y de enfermería, que son muy difíciles de conseguir para profesionales extranjeros. Tienes que pasar exámenes específicos (NCLEX para enfermería, USMLE para medicina), pagar miles de dólares en tasas, validar tus credenciales (proceso que puede llevar 1-2 años).

Pero lo más importante: los colegios profesionales de médicos y enfermeros hacen lobby activamente para mantener estas restricciones. Argumentan que es por "control de calidad", pero la realidad es que es proteccionismo puro. Muchos países tienen sistemas de formación médica excelentes (Alemania, Reino Unido, Canadá, Australia, Filipinas), pero sus profesionales no pueden trabajar fácilmente en Estados Unidos. El resultado es una escasez artificial de trabajadores que mantiene los salarios altísimos, y por tanto los precios hospitalarios también.

**Cosas que NO son el problema (aunque mucha gente las menciona)**

Es importante aclarar qué cosas parecen problemas pero en realidad NO impiden la competencia:

**1. EMTALA (obligación de atender emergencias sin pago garantizado):** Hay una ley federal que obliga a los hospitales con urgencias a atender a todos los pacientes, puedan pagar o no. Suena como un problema, pero no lo es. Si no quieres atender urgencias, simplemente no construyas un servicio de urgencias - puedes hacer un centro de cirugía ambulatoria solo para procedimientos electivos. Y si SÍ decides tener urgencias, aunque tengas que absorber un 10-15% de casos no pagados, si tus costes son 40% más bajos que la competencia, sigues siendo muy rentable. Los seguros pagan tarifas normales, y con costes bajos tienes márgenes enormes incluso absorbiendo casos sin pago.

**2. "Los pacientes de emergencia no pueden comparar precios":** Es verdad que un paciente con infarto no puede ir de hospital en hospital comparando. Pero las aseguradoras SÍ pueden negociar precios fijos por adelantado para cada procedimiento. El paciente no necesita comparar en el momento de la emergencia porque su seguro ya negoció las tarifas. Esto no es una barrera fundamental.

**3. "Construir un hospital es muy caro":** Sí, cuesta entre 100-500 millones de dólares abrir un hospital completo. Pero esto es igual en todo el mundo. Si en México cuesta lo mismo construir un hospital y cobran 5-10 veces menos, mientras que en Estados Unidos los precios son altísimos, el retorno de inversión debería ser MEJOR en Estados Unidos, no peor. El coste de construcción no explica por qué no hay competencia.

**4. Regulación MLR - Medical Loss Ratio (los seguros ganan más cuando los costes son altos):** Hay una ley federal que obliga a las aseguradoras a gastar el 80-85% de las primas en atención médica, dejando solo 15-20% para administración y beneficios. Esto crea un incentivo perverso: si los costes médicos son 100\$, la aseguradora puede quedarse con 15-20\$. Si los costes suben a 200$, puede quedarse con 30-40\$. Mayores costes = mayores beneficios absolutos. Por eso las aseguradoras existentes no luchan agresivamente por bajar precios. PERO hay que aclarar: si una aseguradora necesitara MÁS del 15-20% para administración y beneficios, sería extremadamente ineficiente o estaría estafando a sus clientes. El límite del MLR es razonable como protección al consumidor, quizás podría revisarse, pero no hace imposible la competencia. El problema real es que aunque crees una aseguradora eficiente con costes bajos, los hospitales usarían su chantaje contractual (punto 1 de las barreras reales) para bloquearte. El problema fundamental es el chantaje de los hospitales, no el MLR.

**5. Costes administrativos altísimos (25-30% del gasto total):** Estados Unidos gasta el 25-30% del presupuesto sanitario en burocracia y facturación, mientras que Europa gasta 5-8%. Parece un problema enorme. PERO la solución es simple: integración vertical. Creas tu propio hospital Y tu propia aseguradora. Tu hospital solo factura a UN seguro (el tuyo), tu seguro solo trabaja con UN grupo de hospitales (los tuyos). Sistemas internos simples, sin teatro de autorizaciones previas, sin juegos de códigos de facturación, sin rechazos y apelaciones entre entidades que tú controlas. Kaiser Permanente en Estados Unidos hace exactamente esto y tiene costes administrativos mucho más bajos que los competidores fragmentados. El desperdicio persiste en sistemas fragmentados (100 aseguradoras × 1000 hospitales = 100.000 relaciones de facturación diferentes), pero tú puedes evitarlo con integración vertical. El hecho de que más empresas no hagan esto revela que las OTRAS barreras (CON, chantaje contractual, inmigración) son las que realmente bloquean la competencia.

**En resumen:** Si pudiera cambiar las regulaciones, derogaría las leyes Certificate of Need que permiten a hospitales bloquear nuevos competidores, la prohibición de waivers de responsabilidad civil para permitir negociar límites razonables por contrato, las restricciones de inmigración para trabajadores sanitarios facilitando visas y licencias para profesionales extranjeros, y las restricciones que impiden a Medicare negociar precios agresivamente.

Además, ilegalizaría el chantaje contractual: que un hospital amenace a una aseguradora con "nos vamos de tu red si incluyes a ese competidor barato" debería ser competencia desleal, igual que la colusión para fijar precios o el dumping.

Ahora mismo gastamos cientos de miles de millones al año en abogados, facturación, lobbying y peleándonos entre hospitales, aseguradoras y pacientes, en lugar de curar gente. Tenemos los recursos, la tecnología y los profesionales, pero nos falta un sistema que permita que la competencia funcione. Con las regulaciones correctas podríamos tener los mismos procedimientos a una fracción del coste y liberar ese dinero para investigación, mejores salarios, o devolverlo a las familias. En vez de eso, lo quemamos protegiendo monopolios.