# Knowledge-based recommender systems(funk svd)

## Constraint-based 
  - based on explicitly defined set of recommendation rules.
  - fulfill recommendation rules 

## Case-based 
  - based on different types of similarity measures.
  - retrieve items that are similar tospecified requirements.
  
## Both approaches are similar in their conversationalrecommendation process 
  - users specify the requirements.
  - systems try to identify solutions.
  - if no solution can be found, users change requirements.

## Explicit domain knowledge 
  - Sales knowledge elicitation from domain experts.
  - System mimics the behavior of experienced sales assistant.
  - Best-practice sales interactions.
  - Can guarantee “correct” recommendations (determinism) with respect to expert knowledge.
 
## Conversational interaction strategy.
  - Opposed to one-shot interaction.
  - Elicitation of user requirements. 
  - Transfer of product knowledge (“educating users”).


# Hybridization Recap 

## Limitations and success of hybridization strategies 

Only few works in literature compare strategies from the meta-perspective 

## Empirical findings
  - Monolithic: some preprocessing effort traded for more knowledge.

  - Mixed: simple to enact, works well in practice.

  - Ensemble: requires careful matching of scores from different predictors. 

  - Pipelined: works well for two antithetic approaches.

  - Netflix competition –"stacking" recommender systems.

  - Weighted design based on more than 100 predictors.
      - recommendation functions        
      - Adaptive switching of weights based on user model and parameters.

