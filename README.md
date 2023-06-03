# SEIR Model without Vital Dynamics

Note: This is a similar version to the SEIR model found in the wiki, without the vital dynamics: [SEIR Model](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology#The_SEIR_model). For this homework, we removed the vital dynamics from the model, making it simpler by excluding births and deaths in the population.

## Description

Many infectious diseases have an incubation period before becoming infectious, during which the host cannot yet spread the disease. This delay can be incorporated into the SIR model by introducing a latent/exposed population, denoted as E. Infected individuals (not yet infectious) move from the susceptible population (S) to the latent population (E), and from the latent population (E) to the infectious population (I).

The SEIR model is represented by the following differential equations:

Here are the definitions of the variables:
- `S`: Susceptible population
- `E`: Latent/Exposed population
- `I`: Infectious population
- `R`: Recovered population
- `N`: Total population

The infectious rate, β, controls the spread of the disease and represents the probability of transmitting the disease between susceptible and infectious individuals. The incubation rate, δ, determines the rate at which latent individuals become infectious, with the average duration of incubation being 1/δ. The recovery rate, γ, is determined by the average duration of infection, D, where γ = 1/D.

### Compartmental Models in Epidemiology

Compartmental models are a general technique used for mathematical modeling of infectious diseases. The population is divided into compartments labeled with letters such as S, I, or R, representing Susceptible, Infectious, or Recovered individuals, respectively. People can transition between these compartments based on specific flow patterns.

The origin of compartmental models can be traced back to the early 20th century, with significant contributions from researchers such as Ross, Hudson, Kermack, McKendrick, and Kendall. The SIR model, which consists of Susceptible (S), Infectious (I), and Recovered (R) compartments, is one of the simplest compartmental models and serves as the basis for many derivative models.

These models are typically analyzed using ordinary differential equations (ODEs) to make deterministic predictions. However, they can also be employed with stochastic frameworks to account for randomness, which provides a more realistic but complex analysis.

The SIR model, in particular, is effective in predicting the spread of infectious diseases transmitted between humans, where recovery confers lasting resistance, such as measles, mumps, and rubella.

For more information on compartmental models in epidemiology, you can refer to the [Wikipedia article](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology#The_SEIR_model).

## References

- [SEIR Model on Wikipedia](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology#The_SEIR_model)
- [SEIR Model without Vital Dynamics](https://www.idmod.org/docs/emod/hiv/model-seir.html#seir-without-vital-dynamics)
