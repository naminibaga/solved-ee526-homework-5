Download Link: https://assignmentchef.com/product/solved-ee526-homework-5
<br>
<strong>Problem 1.</strong>

<ul>

 <li>Find the shortest path from start to end in the following figure.</li>

 <li>Find the longest path from start to end in the following figure.</li>

</ul>

<strong>Problem 2. </strong>Consider a MDP with two states S={0, 1}, two actions <em>A </em>= {1<em>,</em>2}, and the follow reward function

<em>sa      </em>1<em>,  </em>(<em>s,a</em>) = (0<em>,</em>1)

<sup>( ) </sup>=4<em>,         </em>(<em>s,a</em>) = (0<em>,</em>2)                                                    (1)

<em>R</em>

3<em>,      </em>(<em>s,a</em>) = (1<em>,</em>1)

2<em>, </em>(<em>s,a</em>) = (1<em>,</em>2)

and the transition probabilities  as follows:

(2)

The other probabilities can be deduced, for example:

<em>.                                                 </em>(3)

<table width="0">

 <tbody>

  <tr>

   <td width="531">The discount factor is</td>

   <td width="93"> </td>

  </tr>

  <tr>

   <td width="531"><em>γ </em>= 3<em>/</em>4<em>.</em></td>

   <td width="93">(4)</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>For the policy <em>π </em>that chooses action 1 in state 0, and action 2 in state 1, find the state value function <em>v</em><em>π</em>(<em>s</em>), by writing out the Bellman’s expectation equation, and solve the equation explicitly.</li>

 <li>For the same policy <em>π</em>, obtain the state value function using iterative update based on the Bellman’s expectation equation. You need to list the first 5 iteration values of <em>v</em>(<em>s</em>).</li>

 <li>For the policy <em>π</em>, calculate the <em>q</em><em>π</em>(<em>s,a</em>) function.</li>

 <li>Based on the value function <em>v</em><em>π</em>(<em>s</em>), obtain an improved policy <em>π</em><sup>′ </sup>based on</li>

</ul>

<em>π</em><sup>′</sup>(<em>s</em>) = argmax<em>q</em><em>π</em>(<em>s,a</em>)<em>.                                                  </em>(5)

<em>a</em>

<ul>

 <li>Obtain the optimal value function <em>v</em>∗(<em>s</em>) using value iteration based on the Bellman’s optimality equation, with all initial values set to 0.</li>

 <li>Obtain the optimal policy.</li>

</ul>

<strong>Problem 3. </strong>Consider a MDP with two states S={0, 1}, two actions <em>A </em>= {1<em>,</em>2}, and the follow reward function

<em>sa      </em>1<em>,  </em>(<em>s,a</em>) = (0<em>,</em>1)

<sup>( ) </sup>=4<em>,         </em>(<em>s,a</em>) = (0<em>,</em>2)                                                    (6)

<em>R</em>

3<em>,      </em>(<em>s,a</em>) = (1<em>,</em>1)

2<em>, </em>(<em>s,a</em>) = (1<em>,</em>2)

and the transition probabilities  as follows:

(7)

The other probabilities can be deduced, for example:

<em>.                                                 </em>(8)

<table width="0">

 <tbody>

  <tr>

   <td width="531">The discount factor is</td>

   <td width="93"> </td>

  </tr>

  <tr>

   <td width="531"><em>γ </em>= 3<em>/</em>4<em>.</em></td>

   <td width="93">(9)</td>

  </tr>

 </tbody>

</table>

Exercise on model-free prediction:

<ul>

 <li>For the policy <em>π </em>that chooses action 1 in state 0, and action 2 in state 1, starting from state 0, generate one episode <em>E </em>of 10000 triplets of (<em>R</em><em>i,S</em><em>i,A</em><em>i</em>), i=0, 2, …, 9999, with <em>R</em><sub>0 </sub>= 0, <em>S</em><sub>0 </sub>= 0.</li>

 <li>Based on the episode <em>E</em>, use Monte Carlo policy evaluation to estimate the value function <em>v</em><em>π</em>(<em>s</em>).</li>

 <li>Based on the episode <em>E</em>, use <em>n</em>-step temporal difference policy evaluation to estimate the value function <em>v</em><em>π</em>(<em>s</em>).</li>

</ul>

Exercise on model-free control:

<ul>

 <li>Use the SARSA algorithm to estimate the optimal action-value function <em>q</em>∗(<em>s,a</em>), by running the algorithm in Sutton and Barto’s book (2nd edition, available online).</li>

 <li>Use the Q-learning algorithm to estimate the optimal action-value function <em>q</em>∗(<em>s,a</em>), by running the algorithm in Sutton and Barto’s book (2nd edition, available online).</li>

</ul>

You only need to simulate one episode. In both cases, you will need to decide an appropriate fixed step-size <em>α</em>, and exploration probability <em>ǫ</em>, and number of time steps in the episode.