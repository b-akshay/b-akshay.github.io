# First post

1. TOC
{:toc}

## Section

First, note that for all $z \in \mathcal{P}$ within the support of $\mu_{\mathcal{P}}$, 
we have $\frac{P^n (z)}{\mu_{\mathcal{P}} (z)} = \text{Pr} (Z \in \mathcal{P})$. 
Therefore, 
$$
\ln \text{Pr} (\frac{1}{Z \in \mathcal{P}})
= \frac{ \mathbb{E}_{Z \sim P^n} [ - \ln \text{Pr} (Z \in \mathcal{P}) \mathbf{1} (Z \in \mathcal{P}) ] }{\text{Pr} (Z \in \mathcal{P})} \\
= \frac{ \mathbb{E}_{Z \sim P^n} [ \ln \frac{\mu_{\mathcal{P}} (Z)}{P^n (Z)} \mathbf{1} (Z \in \mathcal{P}) ] }{\text{Pr} (Z \in \mathcal{P})} \nonumber \\
= \mathbb{E}_{Z \sim \mu_{\mathcal{P}} } [ \ln \frac{\mu_{\mathcal{P}} (Z)}{P^n (Z)} ] \\
= \text{D} ( \mu_{\mathcal{P}} \mid\mid P^n ) 
$$

Furthermore, we have 
$$
\text{D} ( \mu_{\mathcal{P}} \mid\mid P^n ) - \text{D} ( \mu_{\mathcal{P}} \mid\mid \omega_{\mathcal{P}}^n ) \\
= \mathbb{E}_{Z \sim \mu_{\mathcal{P}} } [ \ln \frac{\omega_{\mathcal{P}}^n (Z)}{P^n (Z)} ] \\
= \mathbb{E}_{Z \sim \mu_{\mathcal{P}} } [ \sum_{i=1}^{n} \ln \frac{\omega_{\mathcal{P}} (Z_i)}{P (Z_i)} ] \\
= \sum_{i=1}^{n} \mathbb{E}_{Z \sim \mu_{\mathcal{P}} } [ \ln \frac{\omega_{\mathcal{P}} (Z_i)}{P (Z_i)} ] \\
\stackrel{(a)}{=} \sum_{i=1}^{n} \mathbb{E}_{u \sim \omega_{\mathcal{P}}} [ \ln \frac{\omega_{\mathcal{P}} (u)}{P (u)} ] \\
= \sum_{i=1}^{n} \text{D} ( \omega_{\mathcal{P}} \mid\mid P )
= n \text{D} ( \omega_{\mathcal{P}} \mid\mid P )
$$
Here $(a)$ is because of the definition of the marginal $\omega_{\mathcal{P}}$ of the distribution $\mu_{\mathcal{P}}$. 