In December 2022, CNBC Business New published an article stating that ``Since 2000, public funds diverted to helping build professional sports stadiums and arenas have cost taxpayers \$4.3 billion.''  The proponents of using tax payer money to subsidize big sport venues argue that these venues will bring foot traffic to nearby businesses and so increase their revenue (and as a result, future tax collection). So let's see how we can potentially test that claim.

        There are 121 major sport facilities in the United States: 30 MLB (baseball) stadiums, 29 NBA (basketball) arenas, 31 NFL (football) stadiums, and 31 NHL (hockey) arenas. The types of businesses we are considering are Restaurants, Accommodation, and Other retail and entertainment venues. Imagine that you have the following data for about 30,000 businesses located within a 2 mile radius of each of these sport facilities (all data collected in the same year 2024). Here is a list of variables we can work with:
\begin{itemize}
  \item $BusTraf_i$ is the average weekly number of visits to business $i$.
  \item $SportTraf_i$ is the average weekly number of visits to the closest (to business $i$) sport facility.
  \item $Food_i$: =1 if business $i$ is a restaurant-type business, =0 otherwise.
  \item $Accom_i$: =1 if business $i$ is an accommodation-type business (e.g.~a hotel), =0 otherwise.
  \item $Other_i$: =1 if business $i$ is not a restaurant or accommodation business, =0 otherwise.
  \item $NFL_i$: =1 if the closest (to business $i$) sport facility is an NFL stadium, =0 otherwise.
  \item $NBA_i$: =1 if the closest (to business $i$) sport facility is an NBA arena, =0 otherwise.
  \item $MLB_i$: =1 if the closest (to business $i$) sport facility is an MLB stadium, =0 otherwise.
  \item $NHL_i$: =1 if the closest (to business $i$) sport facility is an NHL arena, =0 otherwise.
\end{itemize}
\pagebreak
So, here is a model that can help us check the claim that sport venue visitors will bring foot traffic to nearby businesses (\textbf{the unit of observation $i$ here is a business}) :
    $$BusTraf_i=\beta_0+\beta_1SportTraf_i+\beta_2Food_i+\beta_3Accom_i+\beta_4NFL_i+\beta_5NBA_i+\beta_6MLB_i+u_i$$
\textbf{Here are your questions and assignments based on that model:}
\begin{enumerate}[(a)]
  \item What are the benchmark (baseline) groups in this model?
  \item If more foot traffic to sport venues indeed brings more visits to local businesses, what should be the sign of $\beta_1$?
  \item Which coefficient do you think is higher: $\beta_4$ or $\beta_5$? Explain.
  \item Modify this model (using interaction terms) so that the effect of sport facility foot traffic on local businesses foot traffic varies with the type of sport played at this facility. Explain how you would test the null hypothesis that sport facilities visit have the same effect on local businesses irrespective of what sport is played there.
  \item Modify this model (using interaction terms) so that the effect of sport facility foot traffic on local businesses foot traffic varies with the type of business. Explain how you would test the null hypothesis that sport facilities visit have the same effect on local businesses irrespective of what type of business it is.
\end{enumerate}
