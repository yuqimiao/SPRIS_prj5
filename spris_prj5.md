# Study design

* A phase III randomized (**1-to-1 ratio**), **stratified**, observer-blinded, placebo-controlled trial at **100 U.S. sites** to demonstrate the efficacy for their developing vaccine. 

* Study period

  * The study consists of 2 periods:
    * vaccine period for 2 injections
    * follow up period: 
      * second injection - 14 days: if the subjects have symptoms/being positive at this period, regard as not at risk and will not contribute to the efficacy calculation
      * 14-28 days: follow up period,

* Define primary outcome

  * Efficacy of the vaccine in preventing the first occurence of symptomatic Covid-19 with onset at least 14 days after the second injection among participants who are seronegative at baseline

  * Using the incidence rate as the measure of risk

  * 

    

  * $$
    VE = 1-\frac{p_1}{p_2}
    $$

    * $p_i$ : the number of new cases during 14-28 days over the total number at risk during 14-28 days in group i
    * $x_i$ cases in group i with $n_i$ samples

* Data collection:

  * collect study subjects with seronegative at baseline $N_0$
  * take 2 covid shots 
  * collect status at day 14 after second shot
  * remove those becoming positive during the 14 days
  * Count new cases during 14-28 days

* Study design

  * Blinding and Randomization procedure
    * The primary blind codes are the group codes, and each vaccine number is the investigational vaccine or control vaccine corresponding to the research number, which is represented by different letters. 
    * The secondary blind codes will uncover the final blind codes, i.e. the vaccine name represented by letters, and the low-dose, medium-dose and high-dose investigational vaccine or control vaccine.
    * Use random number generating process in R(?) to generate random codes 
  *  A stratified block randomization method was used, with study site as the stratification factor and block size in each stratum of 15. 

* Statistical hypothesis

  * $H_0:VE\leq30\%, H_1: VE>30\%$

  * parameters:

  * Test stat: 

    * $$
      Z_L=(\log\hat R-\log R_0)/ \hat \sigma
      $$

    * $$
      N=(Z_\alpha+Z_\beta)^2\frac{q_1/kp_1+q_2/(1-k)p_2}{(\log R_0-\log R)^2}
      $$

* variable parameters:

  * 2-level structure: site(N2 = 50) -> subject(N1 = ?), estimate

    * $$
      \rho = \frac{\sigma_u^2}{\sigma_u^2+\pi^2/3}, \\
      N^{*} = N(1+(50-1)\rho) \\
      $$

    * 

  * loss to follow up rate, $N^{**}= N^{*}\frac{1}{1-\lambda}$ 

  * * 











