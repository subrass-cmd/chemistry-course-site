---
title: "Unit 3: Applications of Thermodynamics"
layout: default
---

{% raw %}
[← Course home](./) · [Download the PDF](assets/pdf/unit3.pdf)
{: .crumbs}

# Unit 3: Applications of Thermodynamics

**Syllabus coverage:** *Gibbs’ Helmholtz equations – Helmholtz energy, Gibbs energy. Standard molar Gibbs energy of formation. Temperature and pressure dependence of free energy. The Clapeyron and Clausius-Clapeyron equation - applications. Partial molar quantities – Gibbs-Duhem equation - physical significance. Variation of chemical potential with temperature and pressure. Maxwell’s relationship.*

<details class="toc" markdown="1"><summary>Contents</summary>

* TOC
{:toc}

</details>

## Learning Objectives

On completing this unit, the student should be able to:

- Define the Helmholtz and Gibbs free energy functions and relate them to maximum obtainable work.

- Apply the Gibbs–Helmholtz equations to relate free energy, enthalpy and their temperature coefficients.

- Use standard Gibbs energies of formation to predict the spontaneity of a reaction.

- Derive and apply the temperature and pressure dependence of Gibbs free energy.

- Derive the Clapeyron and Clausius–Clapeyron equations and apply them to phase-equilibrium problems.

- Define partial molar quantities and apply the Gibbs–Duhem equation.

- Define chemical potential and describe its variation with temperature and pressure.

- Derive Maxwell's thermodynamic relations and use them to connect entropy to measurable P– V–T data.

## List of Symbols and Notation

|**Symbol**|**Meaning**|**SI Unit**|
|---|---|---|
|A|Helmholtz free energy (work function)|J|
|G|Gibbs free energy|J|
|μi|Chemicalpotential of component i|J mol⁻¹|
|X̄i|Partial molarpropertyof component i|(units of Xper mol)|
|ΔGf°|Standard Gibbs energyof formation|kJ mol⁻¹|
|Kp|Equilibrium constant(pressure basis)|dimensionless|
|Tb, Tf|Boiling point, Freezing point|K|
|ΔHvap,ΔHfus|Molar enthalpyof vaporisation, fusion|J mol⁻¹|
|ni|Number of moles of component i|mol|
|R|Universalgas constant|8.314 J K⁻¹ mol⁻¹|

## 1. Helmholtz Energy and Gibbs Energy

Unit II introduced internal energy (E), enthalpy (H) and entropy (S) as the basic thermodynamic state functions. To decide the direction of spontaneous change and the maximum work obtainable from a process without having to track the surroundings separately, two further composite state functions are defined: the Helmholtz free energy (A) and the Gibbs free energy (G). Both combine an energy term with an entropy term and were devised so that spontaneity could be judged from properties of the system alone, under stated constraints.

### 1.1 The Work Function (Helmholtz Free Energy), A

$$
A = E - TS
$$

Since E, T and S are all determined by the state of the system, A is itself a state function. For an isothermal change from state 1 to state 2:

$$
\Delta A = \Delta E - T\Delta S
$$

For a reversible isothermal process, ΔS = qrev/T, so TΔS = qrev, and ΔA = ΔE − qrev. Combining with the First Law, ΔE = qrev − wrev, gives ΔA = (qrev − wrev) − qrev = −wrev, i.e.:

$$
-\Delta A = w_{\text{rev}}\ (\text{max})
$$

Thus the decrease in the work function during any isothermal process gives the maximum total work (both expansion and non-expansion work) that can be obtained from the system. A is the natural thermodynamic potential for processes at constant temperature and volume: dA < 0 for a spontaneous change and dA = 0 at equilibrium, under these conditions.

### 1.2 Gibbs Free Energy, G

$$
G = H - TS = (E + PV) - TS = A + PV
$$

G is likewise a state function. For an isothermal, isobaric change:

$$
\Delta G = \Delta H - T\Delta S = \Delta E + P\Delta V - T\Delta S
$$

Since ΔA = ΔE − TΔS and ΔG = ΔA + PΔV, and −ΔA equals the total maximum work wrev, it follows that:

<p class="eq">Net work (excluding PV work) = wrev − PΔV = −ΔG</p>

In other words, the decrease in Gibbs free energy at constant T and P equals the maximum nonexpansion (net) work obtainable from the system — this could be electrical work (as in a fuel cell or electrochemical cell), surface work, or any other form of useful work apart from simple volume expansion against the atmosphere. Because most chemical reactions of practical interest are carried out at (essentially) constant temperature and pressure, G is by far the most widely used thermodynamic potential in chemistry.

### 1.3 Criteria for Spontaneity and Equilibrium

Combining the First and Second Laws (TdS ≥ dE + PdV for any process, with equality holding only for a reversible change) leads to a complete set of spontaneity criteria, each appropriate to a particular pair of variables held constant:

|**Constant conditions**|**Spontaneous(irreversible)**|**Equilibrium(reversible)**|
|---|---|---|
|E, V|dS > 0|dS = 0|
|S, V|dE < 0|dE = 0|
|S, P|dH < 0|dH = 0|
|T, V|dA < 0|dA = 0|
|T, P|dG < 0|dG = 0|

_In practice, dG < 0 at constant T and P is by far the most commonly applied spontaneity criterion, since most reactions of chemical interest are studied under these conditions._

#### Worked Example 1.1 — Maximum work from ΔA
{: .example}

For an isothermal reversible process at 298 K, ΔE = −150 kJ and ΔS = +120 J K ⁻ ¹. ΔA = ΔE − TΔS = −150 000 − 298(120) = −150 000 − 35 760 = −185 760 J = −185.76 kJ Maximum work obtainable, wrev(max) = −ΔA = +185.76 kJ

#### Worked Example 1.2 — Net (non-expansion) work from ΔG
{: .example}

For a reaction at 298 K and 1 atm, ΔH = −285.8 kJ mol⁻¹ and ΔS = −163.4 J K⁻¹ mol⁻¹ (as in H2 + ½O2 → H2O(l)).

ΔG = ΔH − TΔS = −285 800 − 298(−163.4) = −285 800 + 48 693 = −237 107 J ≈ −237.1 kJ mol ⁻ ¹ Since ΔG < 0, the reaction is spontaneous at 298 K, 1 atm, and −ΔG = 237.1 kJ mol⁻¹ is the maximum nonexpansion (e.g. electrical) work obtainable — this is exactly the basis of the H2–O2 fuel cell.

### 1.4 Comparing A and G

|**Feature**|**Helmholtz energy, A**|**Gibbs energy, G**|
|---|---|---|
|Definition|A = E − TS|G = H − TS|
|Natural constraint|Constant T and V|Constant T and P|
|Physical meaning of<br>−Δ(function)|Maximum TOTAL work (incl. PV<br>work)|Maximum NET (non-expansion)<br>work|
|Typical use|Closed rigid vessels; statistical<br>mechanics|Ordinary laboratory reactions,<br>phase and chemical equilibrium|

#### Worked Example 1.3 — Distinguishing total work and net work
{: .example}

For an isothermal process at 298 K with ΔE = −20.0 kJ and ΔS = +40 J K⁻¹, the process also involves an expansion of 2.0 L against a constant external pressure of 1 atm.

ΔA = ΔE − TΔS = −20 000 − 298(40) = −20 000 − 11 920 = −31 920 J; so wrev(max, total) = −ΔA = +31 920 J

PΔV (expansion work) = (1 atm)(2.0 L) = 202.6 J (using 1 L·atm = 101.3 J)

Net (non-expansion) work = wrev(max) − PΔV = 31 920 − 202.6 ≈ 31 717 J, which is exactly −ΔG for the same process (since ΔG = ΔA + PΔV) — confirming that A gives the maximum total work while G gives only the 'useful' work left over after allowing for simple volume expansion.

## 2. Gibbs–Helmholtz Equations

The Gibbs–Helmholtz equations, due to J. W. Gibbs and H. von Helmholtz, connect the free energy of a system with its enthalpy (or internal energy) and the way free energy varies with temperature. Their principal use is to calculate the heat of a reaction (ΔH) from free energy values (ΔG) measured at two different temperatures, or conversely.

### 2.1 Derivation in Terms of G and H (Constant Pressure)

From the combined statement of the First and Second Laws for a closed system doing only PV work, the total differential of G can be shown to be:

$$
dG = V\,dP - S\,dT
$$

At constant pressure (dP = 0), this reduces to dG = −SdT, so:

$$
\left(\frac{\partial G}{\partial T}\right)_P = -S
$$

Applying this relation to the initial and final states of a process and subtracting gives, for the change ΔG = G2 − G1:

$$
\left[\frac{\partial (\Delta G)}{\partial T}\right]_P = -\Delta S
$$

Now, from the definition of Gibbs energy, ΔG = ΔH − TΔS, so ΔS = (ΔH − ΔG)/T. Substituting:

<p class="eq">[∂(ΔG)/∂T]P = (ΔG − ΔH)/T</p>

Rearranging gives the Gibbs–Helmholtz equation in its standard form:

$$
\Delta G = \Delta H + T\left[\frac{\partial (\Delta G)}{\partial T}\right]_P
$$

### 2.2 Derivation in Terms of A and E (Constant Volume)

An exactly parallel derivation, starting from A = E − TS and dA = −SdT at constant volume, gives the analogous relation for processes at constant volume:

<p class="eq">ΔA = ΔE + T [∂(ΔA)/∂T]V</p>

### 2.3 Using the Gibbs–Helmholtz Equation

If ΔG is known at two temperatures T1 and T2 that are reasonably close together, the temperature coefficient (∂ΔG/∂T)P can be approximated as (ΔG2 − ΔG1)/(T2 − T1), and this, together with either ΔG1 or ΔG2, allows ΔH to be calculated (assumed constant over the small temperature interval). Conversely, if ΔH and ΔG are both known at one temperature, the equation gives the slope (∂ΔG/∂T)P directly, which may then be used to estimate ΔG at a nearby temperature.

#### Worked Example 2.1 — Estimating ΔG at a new temperature
{: .example}

For H2(g) + ½O2(g) → H2O(l): ΔH = −68.32 kcal, ΔG = −56.69 kcal at 298 K. Estimate ΔG at 303 K. −56.69 = −68.32 + 298(∂ΔG/∂T)P  ⇒ (∂ΔG/∂T)P = 11.63/298 = 0.0390 kcal K ⁻ ¹ Assuming this slope is constant over a small interval: ΔG(303 K) = −68.32 + 303×0.0390 = −56.50 kcal

#### Worked Example 2.2 — ΔH from ΔG at two temperatures
{: .example}

For N2(g) + 3H2(g) → 2NH3(g): ΔG = −33.089 kJ at 298 K and ΔG = −28.018 kJ at 308 K. Find ΔH. (∂ΔG/∂T)P ≈ (ΔG2 − ΔG1)/(T2 − T1) = [−28.018 − (−33.089)]/(308−298) = 5.071/10 = 0.5071 kJ K ⁻ ¹ Using ΔG = ΔH + T(∂ΔG/∂T)P at 308 K: −28.018 = ΔH + 308(0.5071) ⇒ ΔH = −28.018 − 156.19 = −184.2 kJ

### 2.4 Alternative (1/T) Form of the Gibbs–Helmholtz Equation

A second, very convenient, form of the Gibbs–Helmholtz equation is obtained by considering the quantity ΔG/T rather than ΔG itself. Differentiating ΔG/T with respect to T at constant pressure, using the quotient rule:

<p class="eq">[∂(ΔG/T)/∂T]P = (1/T)(∂ΔG/∂T)P − ΔG/T²</p>

Substituting (∂ΔG/∂T)P = (ΔG − ΔH)/T (from Section 2.1) into the right-hand side:

<p class="eq">[∂(ΔG/T)/∂T]P = (ΔG − ΔH)/T² − ΔG/T² = − ΔH/T²</p>

Since d(1/T) = −dT/T², this is equivalent to the compact and widely used alternative form:

<p class="eq">[∂(ΔG/T)/∂(1/T)]P = ΔH</p>

This form is especially convenient graphically: a plot of ΔG/T against 1/T is a straight line of slope ΔH (over a temperature range in which ΔH may be treated as constant), so ΔH can be obtained directly from experimental ΔG values at several temperatures without restricting the calculation to just two data points.

**Worked Example 2.3 — Using the 1/T form**

ΔG values for a reaction are −40.0 kJ at 300 K and −37.0 kJ at 320 K. Estimate ΔH using the (ΔG/T) vs (1/T) form.

ΔG/T at 300 K = −40 000/300 = −133.33 J K ⁻ ¹;  ΔG/T at 320 K = −37 000/320 = −115.63 J K ⁻ ¹ 1/T at 300 K = 3.333×10 ⁻ ³ K ⁻ ¹; 1/T at 320 K = 3.125×10 ⁻ ³ K ⁻ ¹

Slope = Δ(ΔG/T)/Δ(1/T) = [−115.63−(−133.33)]/[3.125×10⁻³−3.333×10⁻³] = 17.70/(−2.08×10⁻⁴) ≈ −85 100 J = ΔH ≈ −85.1 kJ

## 3. Standard Molar Gibbs Energy of Formation

The standard Gibbs energy of formation, ΔGf°, is defined as the free energy change when one mole of a compound is formed from its constituent elements, with every species in its standard state (298 K, 1 atm, most stable form). By convention, ΔGf° for an element in its standard state is taken as zero, exactly as for ΔHf°.

### 3.1 Calculating ΔG° of a Reaction

<p class="eq">ΔG° = ΣΔGf°(products) − ΣΔGf°(reactants)</p>

Alternatively, ΔG° may be obtained directly from the standard enthalpy and standard entropy of the reaction:

<p class="eq">ΔG° = ΔH° − TΔS°</p>

A representative selection of standard Gibbs energies of formation (298 K) is given below.

|**Substance**|**ΔGf° / kJ mol⁻¹**|
|---|---|
|H2O(l)|−237.1|
|H2O(g)|−228.6|
|CO2(g)|−394.4|
|CO(g)|−137.2|
|NH3(g)|−16.4|
|CH4(g)|−50.8|
|NO(g)|+86.6|
|C6H6(l)|+124.5|

### 3.2 Sign of ΔG° and Spontaneity

- ΔG° < 0 — the reaction, with all reactants and products in their standard states, is spontaneous as written.

- ΔG° > 0 — the reaction is non-spontaneous as written (the reverse reaction is favoured under standard conditions).

- ΔG° = 0 — reactants and products are in equilibrium under standard conditions.

The magnitude of ΔG° is directly related to the equilibrium constant of the reaction, Kp, through the van't Hoff isotherm relation ΔG° = −RT ln Kp (developed fully in the study of chemical equilibrium); a large negative ΔG° corresponds to a reaction that proceeds essentially to completion, while a large positive ΔG° corresponds to a reaction that scarcely proceeds at all.

#### Worked Example 3.1 — Standard Gibbs energy of reaction
{: .example}

For CO(g) + H2O(g) → H2(g) + CO2(g); ΔGf°(kcal mol ⁻ ¹): CO −32.81, H2O −54.64, CO2 −94.26, H2 0. ΔG° = [0 + (−94.26)] − [(−32.81) + (−54.64)] = −94.26 + 87.45 = −6.81 kcal (spontaneous as written)

#### Worked Example 3.2 — ΔG° from ΔH° and ΔS°
{: .example}

For the vaporisation of water at 373 K, ΔH° = +40.8 kJ mol⁻¹; ΔS° = +109.0 J K⁻¹ mol⁻¹ at the same temperature. ΔG° = ΔH° − TΔS° = 40 800 − 373(109.0) = 40 800 − 40 657 = +143 J mol⁻¹ ≈ 0

ΔG° ≈ 0 confirms that liquid and vapour are essentially in equilibrium at the normal boiling point, as expected.

### 3.3 Effect of Temperature on Spontaneity — the Four Sign Combinations

Since ΔG = ΔH − TΔS, the way spontaneity depends on temperature can be summarised for the four possible combinations of the signs of ΔH and ΔS:

|**ΔH**|**ΔS**|**ΔG = ΔH − TΔS**|**Spontaneity**|
|---|---|---|---|
|Negative|Positive|Always negative|Spontaneous at all temperatures|
|Positive|Negative|Alwayspositive|Non-spontaneous at all temperatures|
|Negative|Negative|Negative onlyif T < ΔH/ΔS|Spontaneous onlyat low temperature|
|Positive|Positive|Negative onlyif T > ΔH/ΔS|Spontaneous onlyat high temperature|

#### Worked Example 3.3 — Temperature at which a reaction becomes spontaneous
{: .example}

For a reaction, ΔH = +45.0 kJ mol ⁻ ¹ and ΔS = +125 J K ⁻ ¹ mol ⁻ ¹ (both positive — case 4 in the table above). The reaction becomes spontaneous once T exceeds ΔH/ΔS = 45 000/125 = 360 K. At 298 K (below 360 K), ΔG = 45 000 − 298(125) = 45 000 − 37 250 = +7750 J > 0, so the reaction is nonspontaneous at room temperature but becomes spontaneous on heating above 360 K — a pattern typical of endothermic decompositions and phase changes.

## 4. Temperature and Pressure Dependence of Free Energy

The two partial derivatives of G with respect to temperature and pressure follow directly from the combined statement of the First and Second Laws, dG = VdP − SdT, applied to a closed system doing only PV work:

<p class="eq">(∂G/∂T)P = − S               (∂G/∂P)T = V</p>

Since entropy S is always positive, G decreases as temperature rises at constant pressure. Since molar volume V is always positive, G increases as pressure rises at constant temperature. Gases, having much larger molar volumes than liquids or solids, show a correspondingly much stronger dependence of G on pressure.

### 4.1 Isothermal Change of G with Pressure — Ideal Gas

At constant temperature, dG = VdP. For n moles of an ideal gas, V = nRT/P, so:

<p class="eq">dG = nRT (dP/P)</p>

Integrating between P1 and P2:

<p class="eq">ΔG = nRT ln(P2/P1) = 2.303 nRT log(P2/P1) = 2.303 nRT log(V1/V2)</p>

**Worked Example 4.1 — ΔG for isothermal expansion**

4 mol of an ideal gas expand isothermally from 1 L to 10 L at 300 K. ΔG = 2.303 nRT log(V1/V2) = 2.303 × 4 × 8.314 × 300 × log(1/10) = 22 976.5 × (−1) = −22 976.5 J = −22.98 kJ

#### Worked Example 4.2 — ΔG for isothermal compression
{: .example}

2 mol of an ideal gas expand reversibly and isothermally at 300 K from 0.1 atm to 1 atm. ΔG = 2.303 nRT log(P2/P1) = 2.303 × 2 × 8.314 × 300 × log(1/0.1) = 11 488.2 × (+1) = +11 488.2 J = +11.49 kJ

The positive ΔG confirms that compression to a higher pressure at constant temperature is the nonspontaneous (free-energy-increasing) direction, requiring work to be done on the gas.

### 4.2 Combining the T and P Dependences — the Gibbs–Helmholtz Route

Because (∂G/∂T)P = −S and G = H − TS, eliminating S between these two relations reproduces exactly the Gibbs–Helmholtz equation of Section 2.1 — the temperature dependence of G is therefore not an independent fact but a direct consequence of the definitions of G, H and S, and this internal consistency is one of the most elegant features of classical thermodynamics.

### 4.3 Free Energy Change for a Solid or Liquid under Pressure

Because the molar volume of a solid or liquid changes only slightly with pressure, ΔG for a condensed phase subjected to a pressure change ΔP is well approximated by ΔG ≈ VΔP (V taken as essentially constant), in contrast with a gas, whose much larger and more pressure-sensitive volume requires the full logarithmic expression derived above.

## 5. The Clapeyron Equation

The Clapeyron equation is an exact thermodynamic relation giving the slope of the equilibrium curve (dP/dT) between any two phases of a pure substance, in terms of the enthalpy and volume changes of the transition.

### 5.1 Derivation

Consider one mole of a liquid (molar volume V1) in reversible equilibrium with its vapour (molar volume V2) at pressure P and temperature T:

<p class="eq">Liquid ⇌ Vapour</p>

Allow the liquid to evaporate reversibly at constant T; the work done during vaporisation is w = P(V2 − V1). Differentiating with respect to temperature (holding V2 − V1 fixed for this step):

<p class="eq">dw/dT = (dP/dT)(V2 − V1)</p>

The heat absorbed in this reversible, constant-temperature vaporisation is the molar latent heat, ΔH, so from the First Law, ΔE = w − ΔH. Substituting into the Gibbs–Helmholtz-type relation for this phase change (obtained by applying the Gibbs–Helmholtz treatment to this isothermal transition) and simplifying gives:

<p class="eq">ΔH = T(V2 − V1)(dP/dT)</p>

Rearranged, this is the Clapeyron equation, applicable in general to any two-phase equilibrium of a pure substance (solid–liquid, liquid–vapour or solid–vapour):

<p class="eq">dP/dT = ΔH / [T(V2 − V1)]</p>

Here ΔH is the molar enthalpy of the transition and (V2 − V1) is the corresponding molar volume change (final phase minus initial phase).

### 5.2 Application to Solid–Liquid Equilibrium

For fusion, ΔV = Vliquid − Vsolid is usually small and can be positive or negative (water is the classic exception, where ice is less dense than liquid water, so Vliquid < Vsolid and dP/dT is negative — the melting point of ice is lowered by increased pressure). For most other substances, Vliquid > Vsolid and dP/dT is positive, so increased pressure raises the melting point.

#### Worked Example 5.1 — Effect of pressure on the melting point of ice
{: .example}

For ice → water at 273 K: ΔHfusion = 6007.8 J mol⁻¹; molar volumes, water 0.018 dm³ mol⁻¹, ice 0.0196 dm³ mol ⁻ ¹ (ΔV = −0.0016 dm³ mol ⁻ ¹, i.e. −1.6×10 ⁻ ⁶ m³ mol ⁻ ¹).

dP/dT = ΔH/(TΔV) = 6007.8/(273 × (−1.6×10 ⁻ ⁶)) ≈ −1.37×10⁷ Pa K ⁻ ¹ ≈ −135 atm K ⁻ ¹

Equivalently dT/dP ≈ −0.0074 K atm⁻¹: an increase of about 135 atm is needed to lower the melting point of ice by just 1 K — the negative sign correctly reflects that increasing pressure lowers the melting point of ice.

#### Worked Example 5.2 — Rate of change of boiling point with pressure
{: .example}

For water at its normal boiling point (373 K, 1 atm), ΔHvap = 40 700 J mol⁻¹; molar volume of vapour ≈ RT/P = (8.314×373)/(1.013×10⁵) = 0.0306 m³ mol ⁻ ¹ (liquid volume negligible in comparison). dP/dT = ΔH/[T(V2−V1)] ≈ 40 700/(373×0.0306) = 40 700/11.41 ≈ 3567 Pa K ⁻ ¹ ≈ 0.0352 atm K ⁻ ¹

This shows that the boiling point of water rises by roughly 1 K for every ≈28 mmHg (≈0.037 atm) rise in the applied pressure near 373 K — consistent with the operating principle of a pressure cooker.

## 6. The Clausius–Clapeyron Equation and its Applications

For liquid–vapour or solid–vapour equilibria, two simplifications can be made to the general Clapeyron equation: (i) the volume of the condensed phase (V1) is negligible compared with the volume of the vapour (V2), so V2 − V1 ≈ V2; and (ii) the vapour is assumed to obey the ideal gas law, V2 = RT/P (per mole).

### 6.1 Derivation

Substituting these approximations into the Clapeyron equation:

<p class="eq">dP/dT = ΔH·P / (RT²)</p>

Rearranging and using d(ln P)/dP = 1/P:

<p class="eq">d(ln P)/dT = ΔH / (RT²)</p>

This differential form is the Clausius–Clapeyron equation. If ΔH (the molar heat of vaporisation, assumed constant over the temperature range of interest) is known, direct integration gives:

<p class="eq">ln P = − ΔH/(RT) + constant</p>

Evaluating this expression at two temperatures T1 and T2 (vapour pressures P1 and P2) and subtracting eliminates the constant, giving the integrated Clausius–Clapeyron equation used in numerical work:

<p class="eq">log(P2/P1) = [ΔH / (2.303 R)] × [(T2 − T1)/(T1 T2)]</p>

### 6.2 Applications

#### (a) Calculation of the Latent Heat of Vaporisation

Given the vapour pressure of a liquid at two different temperatures, ΔH can be calculated directly from the integrated equation.

**Worked Example 6.1 — Latent heat from vapour pressure data**

Vapour pressures of water are 634 mmHg at 368 K and 760 mmHg at 373 K. Find ΔHvap. log(760/634) = [ΔH/(2.303×1.987)] × [(373−368)/(368×373)] log(1.199) = 0.0788 = [ΔH/4.576] × [5/137 264] = ΔH × 7.96×10 ⁻ ⁶ ΔH ≈ 9886 cal mol⁻¹

#### (b) Calculation of Boiling Point (or Freezing Point) at a New Pressure

#### Worked Example 6.2 — Boiling point at reduced pressure
{: .example}

At what temperature will water boil at a hill station where atmospheric pressure is 500 mmHg? (ΔHvap = 2.3 kJ g ⁻ ¹ = 41.4 kJ mol ⁻ ¹; R = 8.314 J K ⁻ ¹ mol ⁻ ¹; normal boiling point 373 K at 760 mmHg.) ln(760/500) = (41 400/8.314)[(1/T2) − (1/373)] 0.4183 = 4980.5 × [(1/T2) − 0.002681] (1/T2) = 0.002681 + 8.40×10⁻⁵ = 0.002765 ⇒ T2 ≈ 361.7 K (≈ 88.5 °C) — boiling occurs at a lower temperature, as expected at reduced pressure.

#### (c) Calculation of Vapour Pressure at a New Temperature

#### Worked Example 6.3 — Vapour pressure at a lower temperature
{: .example}

Vapour pressure of water at 100 °C is 76.0 cm. Estimate its vapour pressure at 90 °C, given mean ΔHvap = 542 cal g ⁻ ¹ (= 9756 cal mol ⁻ ¹) over this range.

log(P2/76.0) = [9756/(2.303×1.987)] × [(363−373)/(363×373)]

log(P2/76.0) = 2129.5 × (−7.386×10 ⁻ ⁵) = −0.1573 P2/76.0 = 0.696 ⇒ P2 ≈ 52.9 cm — vapour pressure falls, as expected on cooling.

#### (d) Molal Elevation and Molal Depression Constants

Applying the Clausius–Clapeyron equation to the small change in vapour pressure caused by dissolving a solute (via Raoult's Law), together with the definitions of the molal elevation constant, Kb (elevation in boiling point per mole of solute per kg of solvent), and the molal depression constant, Kf, gives:

<p class="eq">Kb = 0.002 Tb² / lvap        Kf = 0.002 Tf² / lfus</p>

where lvap and lfus are the latent heats of vaporisation and fusion of the solvent per gram, and Tb, Tf its boiling and freezing points (K).

#### Worked Example 6.4 — Molal depression constant of water
{: .example}

Latent heat of fusion of ice = 80 cal g ⁻ ¹; freezing point of water = 273 K. Kf = 0.002 × 273² / 80 = 0.002 × 74 529/80 = 1.86 K per 1000 g of water — the well-known cryoscopic constant of water.

#### (e) Trouton's Rule — a Useful Empirical Cross-Check

Since ΔSvap = ΔHvap/Tb (Unit II, Section 9.5), and the Clausius–Clapeyron equation shows ΔHvap governs how strongly vapour pressure varies with temperature, it is not surprising that ΔSvap itself is found empirically to be roughly constant (≈ 85–90 J K⁻¹ mol⁻¹) for a great many normal (nonassociated, non-polar) liquids at their boiling points — an empirical observation known as Trouton's Rule. It provides a quick, approximate way of estimating ΔHvap = Tb × ΔSvap when only the boiling point is known, and conversely, a liquid whose ΔSvap departs substantially from this range (e.g. water, ΔSvap ≈ 109 J K⁻¹ mol⁻¹) can be inferred to show significant association (hydrogen bonding) in the liquid state.

#### Worked Example 6.5 — Estimating ΔHvap using Trouton's Rule
{: .example}

Estimate ΔHvap for benzene (Tb = 353 K) using Trouton's Rule (ΔSvap ≈ 88 J K⁻¹ mol⁻¹), and compare with the literature value of 30.8 kJ mol ⁻ ¹.

ΔHvap(estimated) = Tb × ΔSvap = 353 × 88 = 31 064 J mol ⁻ ¹ ≈ 31.1 kJ mol ⁻ ¹

This is within about 1% of the literature value, illustrating the good reliability of Trouton's Rule for a 'normal' (non-associated) liquid such as benzene.

## 7. Partial Molar Quantities

The thermodynamic relations developed so far (in Units II and III) apply strictly to closed systems of fixed composition. To describe mixtures and solutions — open systems in which composition, as well as temperature and pressure, can vary — G. N. Lewis introduced the concept of partial molar properties.

### 7.1 Definition

Consider an extensive property X (e.g. volume, enthalpy, Gibbs energy) of a mixture containing n1, n2, …, nj moles of its various constituents; X depends on T, P and all the ni. The partial molar property of component i is defined as the rate of change of X with ni, holding T, P and the amounts of all other constituents constant:

<p class="eq">X̄i = (∂X/∂ni)T,P,nj (j≠i)</p>

Physically, X̄i represents the contribution that one mole of component i makes to the total extensive property X of the mixture, under the given conditions of temperature, pressure and composition — this contribution is not, in general, equal to the molar property of pure i, because of interactions between unlike molecules in the mixture.

### 7.2 Additivity of Partial Molar Properties

For a mixture of fixed (definite) composition, integrating the total differential of X (at constant T and P, where dT = dP = 0) shows that the partial molar properties combine simply as a mole-weighted sum:

$$
X = n_1\bar{X}_1 + n_2\bar{X}_2 + \dots + n_j\bar{X}_j
$$

The most important partial molar property in chemical thermodynamics is the partial molar Gibbs free energy, which is identical to the chemical potential (introduced formally in Section 9).

### 7.3 Partial Molar Volume — a Worked Illustration

The partial molar volume of component i, V̄i = (∂V/∂ni)T,P,nj, illustrates the concept concretely: when a small amount of ethanol is added to a large volume of water, the total volume of the mixture increases by less than the volume of pure ethanol added, because ethanol molecules pack more efficiently among the hydrogen-bonded water molecules than they do in pure ethanol. The partial molar volume of ethanol in this dilute aqueous solution is therefore smaller than its molar volume as a pure liquid. Partial molar volumes are generally obtained experimentally from the slope of a plot of the measured total volume of solutions of varying composition against the number of moles of the component of interest, at constant T, P and the amount of the other component(s).

#### Worked Example 7.1 — Estimating a partial molar volume from experimental data
{: .example}

The total volume of a solution containing 1 kg of water and n2 mol of a solute is found (over a small range) to fit V = 1003 + 18.5 n2 (V in cm³, n2 in mol). Find the partial molar volume of the solute. V ̄ 2 = (∂V/∂n2)T,P,n1 = 18.5 cm³ mol⁻¹ (the coefficient of n2 in the fitted expression, since it is already linear in n2 over the range considered).

This value is the partial molar volume of the solute in this particular (dilute) aqueous solution; it need not equal the molar volume of the pure solute, precisely because of solute–solvent interactions in solution, as emphasised in Section 7.1.

## 8. The Gibbs–Duhem Equation

The Gibbs–Duhem equation expresses an important constraint linking the partial molar properties (in particular, the chemical potentials) of the different components of a mixture at constant temperature and pressure.

### 8.1 Derivation

The total Gibbs energy of a mixture, expressed in terms of the number of moles and chemical potentials of its components, is G = Σ ni μi. Taking the total differential of this expression:

$$
dG = \sum \mu_i\,dn_i + \sum n_i\,d\mu_i
$$

But the general total differential of G for an open system, in terms of T, P and composition, is also known to be:

$$
dG = -S\,dT + V\,dP + \sum \mu_i\,dn_i
$$

Comparing the two expressions for dG (they must be identical) shows that, at constant temperature and pressure (dT = dP = 0):

<p class="eq">Σ ni dμi = 0     (Gibbs–Duhem equation, constant T and P)</p>

### 8.2 Physical Significance

The Gibbs–Duhem equation shows that the chemical potentials (and, more generally, the partial molar properties) of the different components of a mixture cannot vary independently of one another at constant temperature and pressure: a change in the chemical potential of one component must be accompanied by a compensating change in that of the other component(s), weighted by their respective mole numbers. For a two-component (binary) mixture, this is often written:

$$
n_1\,d\mu_1 + n_2\,d\mu_2 = 0 \quad\Longrightarrow\quad d\mu_2 = -\frac{n_1}{n_2}\,d\mu_1
$$

This relation is of substantial practical importance: it allows the chemical potential (or activity) of one component of a binary solution to be calculated from experimental measurements made only on the other component, without needing to determine both independently. This technique is widely used, for example, in obtaining the activity of a non-volatile solute from vapour-pressure (activity) measurements of the volatile solvent.

#### Worked Example 8.1 — Illustrating the Gibbs–Duhem constraint
{: .example}

In a binary mixture of components 1 and 2 with n1 = 2 mol and n2 = 8 mol, if μ1 is found (experimentally) to increase by 500 J mol ⁻ ¹ over a small composition change, estimate the corresponding change in μ2. From n1dμ1 + n2dμ2 = 0: dμ2 = −(n1/n2)dμ1 = −(2/8)(500) = −125 J mol ⁻ ¹

As μ1 increases, μ2 must decrease, and by a smaller amount because component 2 is present in greater quantity — illustrating the compensating nature of the Gibbs–Duhem relation.

## 9. Chemical Potential

The chemical potential is one of the most important quantities in chemical thermodynamics, providing the criterion for equilibrium and the direction of spontaneous change in systems where matter, not just energy, can be redistributed (between phases, or through a chemical reaction).

### 9.1 Definition

The chemical potential of component i, μi, is defined as its partial molar Gibbs free energy:

<p class="eq">μi = (∂G/∂ni)T,P,nj (j≠i)</p>

Physically, μi represents the increase in the total Gibbs free energy of a (large) system when one mole of component i is added at constant temperature and pressure, without appreciably altering the overall composition.

### 9.2 Physical Significance — Escaping Tendency

The chemical potential may usefully be thought of as the escaping tendency of a substance from a given phase or state: matter flows spontaneously from a region (or phase) of high chemical potential to one of low chemical potential, exactly as heat flows spontaneously from high to low temperature, and electric charge flows from high to low electrical potential. At equilibrium, the chemical potential of any given substance must be identical in every phase (or location) in which that substance is present — this is the general equilibrium condition for multi-phase and multi-component systems, and underlies phenomena such as vapour–liquid equilibrium, solubility equilibria and membrane equilibria.

### 9.3 Variation of Chemical Potential with Temperature

Differentiating μi = (∂G/∂ni)T,P with respect to T, and using the general relation (∂G/∂T)P = −S together with the definition of a partial molar property, gives:

<p class="eq">(∂μi/∂T)P = − S̄i     (S̄i = partial molar entropy of component i)</p>

Since S̄i is always positive, the chemical potential of every substance decreases as temperature increases at constant pressure — exactly analogous to the behaviour of the molar Gibbs energy of a pure substance.

### 9.4 Variation of Chemical Potential with Pressure

Similarly, differentiating with respect to pressure and using (∂G/∂P)T = V together with the partial molar property definition:

<p class="eq">(∂μi/∂P)T = V̄i     (V̄i = partial molar volume of component i)</p>

Since V̄i is always positive, the chemical potential of a substance increases as pressure increases at constant temperature. For an ideal gas, integrating this relation from a standard pressure P° (usually 1 atm) to any pressure P gives the very useful explicit expression:

$$
\mu_i = \mu_i^\circ + RT\ln\frac{P}{P^\circ}
$$

where μi° is the chemical potential of the pure gas i at the standard pressure P° and the same temperature. This expression is the starting point for the thermodynamic treatment of gaseous equilibria (developed in the study of chemical equilibrium) and for the definition of activity in nonideal systems.

#### Worked Example 9.1 — Chemical potential of an ideal gas at a new pressure
{: .example}

Estimate the change in chemical potential of an ideal gas at 298 K when its pressure is increased from 1 atm to 5 atm.

Δμ = RT ln(P2/P1) = 8.314 × 298 × ln5 = 2477.6 × 1.609 = 3987.6 J mol ⁻ ¹ ≈ +3.99 kJ mol ⁻ ¹ The chemical potential — and hence the escaping tendency — of the gas increases substantially on compression, consistent with the tendency of a compressed gas to expand spontaneously when released.

### 9.5 Chemical Potential as a General Equilibrium Criterion

The equal-chemical-potential condition developed above is completely general and underlies several important equilibria beyond simple liquid–vapour phase equilibrium:

- Solubility equilibrium: a solid solute in contact with a saturated solution is at equilibrium when the chemical potential of the solute in the solid phase equals its chemical potential in solution; if the solution is unsaturated, the solute's chemical potential in the solid exceeds that in solution, and dissolution proceeds spontaneously (matter flows from high to low chemical potential) until the two become equal.

- Distribution between immiscible solvents: when a solute distributes itself between two immiscible liquid layers in contact, equilibrium is reached when the chemical potential of the solute is the same in both layers — this is the thermodynamic basis of the distribution (partition) law encountered in solvent-extraction techniques.

- Membrane and osmotic equilibrium: solvent flows across a semi-permeable membrane from the side of higher solvent chemical potential (pure solvent) to the side of lower solvent chemical potential (solvent in solution) until the chemical potentials on the two sides become equal, which is the origin of osmotic pressure.

_In every case, the underlying principle is identical: at equilibrium, the chemical potential of any freely mobile species must be the same throughout all the regions (phases) accessible to it._

## 10. Maxwell's Relations

Maxwell's relations are a set of four equations connecting the partial derivatives of P, V, T and S. They are derived from the four thermodynamic potentials — internal energy (E), enthalpy (H), Helmholtz energy (A) and Gibbs energy (G) — using the mathematical fact that each of these is a true state function, so that its total differential is exact and its mixed second partial derivatives must be equal (Euler's reciprocity theorem).

### 10.1 The Four Fundamental (Combined Law) Equations

For a closed system doing only PV work, combining the First Law (dE = dq − PdV) with the Second Law (dq = TdS for a reversible change) gives the master equation dE = TdS − PdV. The corresponding expressions for H, A and G follow immediately from their definitions:

$$
dE = T\,dS - P\,dV
$$

$$
\begin{aligned} dH &= d(E + PV) = T\,dS + V\,dP \\ dA &= d(E - TS) = -S\,dT - P\,dV \\ dG &= d(H - TS) = -S\,dT + V\,dP \end{aligned}
$$

### 10.2 The Reciprocity (Euler) Condition

For any exact differential of the form dZ = M(x,y) dx + N(x,y) dy, the mixed second partial derivatives of Z must be equal regardless of the order of differentiation:

$$
\left(\frac{\partial M}{\partial y}\right)_x = \left(\frac{\partial N}{\partial x}\right)_y
$$

Applying this reciprocity condition in turn to each of the four fundamental equations above yields the four Maxwell relations.

### 10.3 Derivation of the Four Maxwell Relations

**_(i) From dE = TdS − PdV_**

Here M = T, N = −P, x = S, y = V. The reciprocity condition (∂M/∂y)x = (∂N/∂x)y gives:

$$
\left(\frac{\partial T}{\partial V}\right)_S = -\left(\frac{\partial P}{\partial S}\right)_V
$$

**_(ii) From dH = TdS + VdP_**

Here M = T, N = V, x = S, y = P:

$$
\left(\frac{\partial T}{\partial P}\right)_S = \left(\frac{\partial V}{\partial S}\right)_P
$$

**_(iii) From dA = − SdT − PdV_**

Here M = −S, N = −P, x = T, y = V:

$$
\left(\frac{\partial S}{\partial V}\right)_T = \left(\frac{\partial P}{\partial T}\right)_V
$$

**_(iv) From dG = − SdT + VdP_**

Here M = −S, N = V, x = T, y = P:

$$
\left(\frac{\partial S}{\partial P}\right)_T = -\left(\frac{\partial V}{\partial T}\right)_P
$$

### 10.4 Summary Table of Maxwell's Relations

|**Potential**|**Fundamental equation**|**Maxwell relation obtained**|
|---|---|---|
|E|dE = TdS − PdV|(∂T/∂V)S = −(∂P/∂S)V|
|H|dH = TdS + VdP|(∂T/∂P)S =(∂V/∂S)P|
|A|dA = −SdT − PdV|(∂S/∂V)T =(∂P/∂T)V|
|G|dG = −SdT + VdP|(∂S/∂P)T = −(∂V/∂T)P|

### 10.5 Significance and Applications

The great practical value of Maxwell's relations is that they allow entropy changes — which cannot be measured directly — to be calculated entirely from P–V–T data, which are readily obtained from experiment (e.g. from an equation of state, or from measurements of thermal expansivity and compressibility). For example:

- The relation (∂S/∂V)T = (∂P/∂T)V allows the isothermal variation of entropy with volume to be found purely from how pressure varies with temperature at constant volume.

- The relation (∂S/∂P)T = −(∂V/∂T)P connects the isothermal variation of entropy with pressure to the thermal expansion coefficient of the substance, α = (1/V)(∂V/∂T)P, since (∂S/∂P)T = −Vα.

#### Worked Example 10.1 — Applying a Maxwell relation to an ideal gas
{: .example}

Use the Maxwell relation (∂S/∂V)T = (∂P/∂T)V to find (∂S/∂V)T for one mole of an ideal gas, and hence confirm the entropy formula obtained in Unit II by direct integration.

For an ideal gas, P = RT/V, so (∂P/∂T)V = R/V.

By the Maxwell relation, (∂S/∂V)T = R/V. Integrating at constant T from V1 to V2: ΔS = R ln(V2/V1) — exactly matching the ideal-gas entropy expression derived independently in Unit II (Section 9.3), confirming the internal consistency of the two approaches.

#### Worked Example 10.2 — Using Maxwell's relation with thermal expansivity
{: .example}

For a liquid with thermal expansion coefficient α = 2.1×10⁻⁴ K⁻¹ and molar volume V = 18×10⁻⁶ m³ mol⁻¹ (approximating water near room temperature), estimate (∂S/∂P)T. (∂S/∂P)T = −Vα = −(18×10 ⁻ ⁶)(2.1×10 ⁻ ⁴) = −3.78×10 ⁻ ⁹ m³ K ⁻ ¹ mol ⁻ ¹ (J K ⁻ ¹ Pa ⁻ ¹ mol ⁻ ¹)

The small magnitude confirms that the entropy of a condensed phase is only weakly sensitive to pressure, in sharp contrast with a gas, for which (∂S/∂P)T = −R/P is very much larger at ordinary pressures.

## 11. Relationship Between the Four Thermodynamic Potentials

Internal energy (E), enthalpy (H), Helmholtz energy (A) and Gibbs energy (G) are collectively known as the four thermodynamic potentials. Each is a state function, and each has a particular pair of variables — its natural variables — in terms of which its total differential takes the simplest possible form (as used throughout Section 10).

|**Potential**|**Definition**|**Natural variables**|**Differential form**|
|---|---|---|---|
|Internal energy, E|—|S, V|dE = TdS − PdV|
|Enthalpy, H|H = E + PV|S, P|dH = TdS + VdP|
|Helmholtz energy, A|A = E − TS|T, V|dA = −SdT − PdV|
|Gibbs energy, G|G = H − TS|T, P|dG = −SdT + VdP|

### 11.1 Reading Off T, P and S from the Potentials

From the four differential forms above, each of T, −P and −S can be read off directly as a partial derivative of the appropriate potential with respect to its natural variable, holding the other natural variable fixed:

$$
T = \left(\frac{\partial E}{\partial S}\right)_V = \left(\frac{\partial H}{\partial S}\right)_P
$$

$$
\begin{aligned} -P &= \left(\frac{\partial E}{\partial V}\right)_S = \left(\frac{\partial A}{\partial V}\right)_T \\ -S &= \left(\frac{\partial A}{\partial T}\right)_V = \left(\frac{\partial G}{\partial T}\right)_P \\ V &= \left(\frac{\partial H}{\partial P}\right)_S = \left(\frac{\partial G}{\partial P}\right)_T \end{aligned}
$$

These relations, together with the reciprocity condition applied in Section 10, are the complete source of all four Maxwell relations — in effect, Sections 10 and 11 present two views (differential and tabular) of exactly the same underlying mathematical structure, and together they form a compact 'toolkit' relating the mechanical variables (P, V, T) to the thermal variable (S) through the four energylike potentials (E, H, A, G).

### 11.2 A Memory Aid — the Thermodynamic Square

Students often find it convenient to arrange the four potentials and four natural variables on a simple diagram (the 'thermodynamic square'): the four potentials E, H, G, A are placed on the sides of a square (in the order E, H, G, A reading clockwise from the top-left), with the four natural variables S, P, T, V placed at the corners between the two potentials to which each is natural. Once drawn, the differential relations, the reciprocity (Maxwell) relations, and the sign conventions can all be read directly from the diagram, without needing to re-derive them from first principles in an examination — this is purely a revision aid and does not replace understanding the underlying derivations given in Section 10.

#### Worked Example 11.1 — Using the potential table directly
{: .example}

Given (∂G/∂T)P = −S for a certain substance, and separately that its entropy increases by 12 J K⁻¹ mol⁻¹ when heated by 5 K at constant pressure, estimate the corresponding change in G.

ΔG ≈ (∂G/∂T)P × ΔT = −S × ΔT. Taking S ≈ 150 J K ⁻ ¹ mol ⁻ ¹ (a typical gas-phase value) as representative: ΔG ≈ −150 × 5 = −750 J mol⁻¹ — G decreases as temperature rises, consistent with (∂G/∂T)P = −S always being negative.

## Additional Solved Numerical Problems

The following fully worked problems draw together several concepts from this unit and are recommended for consolidation before attempting the Review Questions.

#### Solved Problem 1 — Free energy, spontaneity and the equilibrium constant link
{: .example}

For a reaction at 298 K, ΔH° = −92.4 kJ mol⁻¹ and ΔS° = −198.6 J K⁻¹ mol⁻¹ (e.g. N2 + 3H2 → 2NH3). Calculate ΔG° and comment on the implied value of Kp.

ΔG° = ΔH° − TΔS° = −92 400 − 298(−198.6) = −92 400 + 59 203 = −33 197 J ≈ −33.2 kJ mol ⁻ ¹

Since ΔG° < 0, ln Kp = −ΔG°/RT is positive, so Kp > 1: the reaction, at equilibrium, favours products under standard conditions at 298 K.

#### Solved Problem 2 — Clapeyron equation applied to sublimation
{: .example}

Estimate d(lnP)/dT for the sublimation of CO2(s) → CO2(g) at 195 K, given ΔHsub = 25.2 kJ mol⁻¹ and assuming the vapour behaves ideally with negligible solid volume.

Using the Clausius–Clapeyron form d(lnP)/dT = ΔH/(RT²): at 195 K, d(lnP)/dT = 25 200/(8.314×195²) = 25 200/316 240 ≈ 0.0797 K ⁻ ¹

This positive value confirms that the sublimation vapour pressure of solid CO2 rises steeply with temperature, consistent with its familiar rapid sublimation on gentle warming.

#### Solved Problem 3 — Combining Gibbs–Helmholtz reasoning with phase equilibrium
{: .example}

Show that, for a pure liquid in equilibrium with its vapour at the normal boiling point, ΔGvap = 0 is consistent with ΔSvap = ΔHvap/Tb.

At the boiling point, liquid and vapour are in equilibrium, so ΔGvap = 0, giving directly ΔHvap = TbΔSvap, i.e. ΔSvap = ΔHvap/Tb — identical to the phase-transition entropy relation of Unit II, confirming that the Gibbs energy criterion for phase equilibrium (ΔG = 0) is fully consistent with the earlier, more elementary entropy-based treatment of phase changes.

#### Solved Problem 4 — Chemical potential and equilibrium between phases
{: .example}

Explain, using chemical potential, why a liquid boils at the temperature at which its vapour pressure equals the external (atmospheric) pressure.

At any temperature, the liquid phase has chemical potential μ(l) and the vapour (at the prevailing partial pressure) has chemical potential μ(g) = μ°(g) + RT ln(P/P°). Boiling — bulk vaporisation throughout the liquid, not just at the surface — occurs when μ(l) = μ(g), i.e. when the vapour pressure of the liquid has risen (with increasing temperature) to equal the external pressure, so that vapour can form freely against that pressure; below this temperature μ(l) < μ(g) at the external pressure and no bulk vaporisation occurs, only surface evaporation.

#### Solved Problem 5 — Gibbs–Duhem consistency check for a binary mixture
{: .example}

In a binary mixture, the activity coefficient of component 1, γ1, is found experimentally to fit ln γ1 = k x2² over a range of composition (k a constant, x2 the mole fraction of component 2). Use the Gibbs–Duhem equation to find the corresponding expression for ln γ2.

The Gibbs–Duhem equation for activity coefficients at constant T, P is x1 d(lnγ1) + x2 d(lnγ2) = 0.

d(lnγ1)/dx1 = d(k x2²)/dx1 = k × 2x2 × (dx2/dx1) = −2kx2 (since x2 = 1−x1, dx2/dx1 = −1)

From Gibbs–Duhem: x1(−2kx2) + x2(dlnγ2/dx1) = 0 ⟹ dlnγ2/dx1 = 2kx1  ⟹  integrating, ln γ2 = k x1² (+ constant, taken as zero so that γ2→1 as x1→0)

This symmetric result (ln γ1 = kx2², ln γ2 = kx1²) is the well-known two-suffix Margules form for a simple non-ideal binary solution, obtained directly by enforcing the Gibbs–Duhem constraint.

**Solved Problem 6 — Combining the Clausius–Clapeyron and Gibbs–Helmholtz viewpoints** The vapour pressure of a solid is 2.0 mmHg at 200 K and 10.0 mmHg at 220 K. Estimate ΔHsub, and comment on how this value could alternatively be obtained from a plot of ΔGsub/T against 1/T for the sublimation equilibrium.

log(10.0/2.0) = [ΔHsub/(2.303×8.314)] × [(220−200)/(200×220)] log(5.0) = 0.699 = [ΔHsub/19.15] × [20/44 000] = ΔHsub × 2.273×10 ⁻ ⁵ ΔHsub ≈ 30 750 J mol ⁻ ¹ ≈ 30.8 kJ mol ⁻ ¹

Since ΔGsub = 0 at any point on the solid–vapour equilibrium line (the two phases are in equilibrium there), the Gibbs–Helmholtz (1/T) form of Section 2.4 cannot directly be applied to ΔGsub itself (which is identically zero along the whole curve); instead, ΔHsub must be obtained from the pressure–temperature data via the Clausius–Clapeyron equation, as done above — illustrating that the two families of equations (Gibbs– Helmholtz and Clausius–Clapeyron) are complementary tools suited to different types of data.

## Appendix — Comprehensive Worked Problem Set

The following extended problems each combine two or more concepts from this unit. They are intended as capstone practice once every section above has been studied, and are pitched at JAM/competitive-examination level.

#### Appendix Problem A1 — Free energy, Gibbs–Helmholtz and phase change together
{: .example}

A certain solid sublimes according to Solid ⇌ Vapour with ΔHsub = 58.2 kJ mol⁻¹, essentially constant over the temperature range of interest. At 250 K, the sublimation pressure is 1.00 mmHg.

1. Use the Clausius–Clapeyron equation to find the sublimation pressure at 260 K.

2. Given that ΔSsub at 250 K is 235 J K⁻¹ mol⁻¹, calculate ΔGsub at 250 K under a vapour pressure of exactly 1.00 mmHg (i.e. under the actual equilibrium pressure at that temperature), and comment on its value.

Solution:

(1) log(P2/1.00) = [58 200/(2.303×8.314)] × [(260−250)/(250×260)] = 3039.6 × (10/65 000) = 0.4676 P2/1.00 = 2.935 ⟹ P2 ≈ 2.94 mmHg — the sublimation pressure roughly triples over this 10 K rise, reflecting the typically strong (exponential) temperature sensitivity of solid–vapour equilibria.

(2) At 250 K, the solid and its vapour ARE in equilibrium at the vapour pressure of 1.00 mmHg (this is, by definition, the sublimation pressure at that temperature). Therefore ΔGsub = 0 exactly at this pressure, consistent with ΔHsub = TΔSsub check: 250×235 = 58 750 J, close to the given ΔHsub = 58 200 J (small discrepancy reflects rounding in the given data) — confirming the internal consistency required at any point on a genuine phase-equilibrium curve.

#### Appendix Problem A2 — Combining Clapeyron and van't Hoff-type reasoning
{: .example}

Explain, using the Clapeyron equation, why the slope of the solid–liquid equilibrium line on a P–T phase diagram is generally very steep (nearly vertical) compared with the liquid–vapour line.

Solution: For fusion, ΔV = Vliquid − Vsolid is typically very small (of the order of 1–10% of the molar volume), whereas ΔHfusion, though smaller than ΔHvap, is still substantial. Since dP/dT = ΔH/(TΔV), a small ΔV in the denominator, combined with a moderate ΔH in the numerator, produces a very large value of dP/dT — a nearly vertical solid–liquid equilibrium line. By contrast, for vaporisation, ΔV = Vvapour − Vliquid is enormous (the vapour occupies a volume many hundreds of times that of the liquid), so despite a larger ΔHvap, the much larger ΔV in the denominator makes dP/dT far smaller — a much shallower liquid–vapour equilibrium line. This single equation, dP/dT = ΔH/(TΔV), therefore accounts for the characteristically different slopes of the two types of equilibrium line seen on any P– T phase diagram.

#### Appendix Problem A3 — Chemical potential, Gibbs–Duhem and partial molar entropy together
{: .example}

For a binary mixture at constant T and P, show that if the partial molar entropy of component 1, S̄1, increases with the mole fraction x1, the Gibbs–Duhem equation requires the partial molar entropy of component 2, S̄2, to change in a specific, related way, and interpret this physically.

Solution: Since S̄i = −(∂μi/∂T)P (Section 9.3), applying the Gibbs–Duhem equation x1 dμ1 + x2 dμ2 = 0 (mole-fraction form, dividing the standard form by total moles) to the temperature derivative at constant composition gives, after differentiating throughout with respect to T at constant P and x1:

<p class="eq">x1 dS̄1 + x2 dS̄2 = 0     (constant T, P)</p>

So dS̄2 = −(x1/x2) dS̄1: if S̄1 increases with x1, S̄2 must decrease, in the same compensating pattern already established for chemical potential itself in Section 8. Physically, this reflects the fact that entropy contributions in a mixture, like all partial molar properties, are constrained by the overall extensive nature of total entropy — one component's contribution cannot rise without the other's falling correspondingly, when weighted by the respective mole fractions.

**Appendix Problem A4 — Full derivation practice: Maxwell relation to heat-capacity relation** Using the Maxwell relation (∂S/∂V)T = (∂P/∂T)V together with the definition Cv = T(∂S/∂T)V, outline how one could show that (∂Cv/∂V)T = T(∂²P/∂T²)V, and state why this result is useful.

Solution: Differentiate Cv = T(∂S/∂T)V with respect to V at constant T:

<p class="eq">(∂Cv/∂V)T = T (∂/∂T)[(∂S/∂V)T]V = T (∂/∂T)[(∂P/∂T)V]V = T (∂²P/∂T²)V</p>

(using the Maxwell relation to replace (∂S/∂V)T by (∂P/∂T)V, then differentiating again with respect to T at constant V, and invoking the equality of mixed partial derivatives to interchange the order of differentiation). This result is useful because it shows that, for any substance obeying an equation of state that is linear in T at constant V (as an ideal gas does, P = RT/V, giving ∂²P/∂T² = 0), Cv is completely independent of volume — recovering, from purely thermodynamic reasoning (with no molecular assumptions), the familiar ideal-gas result that Cv depends on temperature alone, not on volume or pressure.

**Appendix Problem A5 — Standard Gibbs energies and a two-step reaction pathway**

Given ΔGf°(kJ mol⁻¹): NO(g) +86.6, NO2(g) +51.3, N2(g) 0, O2(g) 0. Calculate ΔG° for (a) N2(g) + O2(g) → 2NO(g), (b) 2NO(g) + O2(g) → 2NO2(g), and (c) the overall reaction N2(g) + 2O2(g) → 2NO2(g) obtained by adding (a) and (b). Verify that ΔG° for the overall reaction equals the sum of the two step values, illustrating that ΔG°, like ΔH°, is a state function and obeys a Hess's-Law-type additivity.

Solution:

(a) ΔG°(a) = 2(86.6) − [0+0] = +173.2 kJ

(b) ΔG°(b) = 2(51.3) − [2(86.6)+0] = 102.6 − 173.2 = −70.6 kJ

(c) Adding (a) and (b) directly: ΔG°(a)+ΔG°(b) = 173.2 + (−70.6) = +102.6 kJ

Direct calculation of (c): ΔG°(c) = 2(51.3) − [0+0] = +102.6 kJ — exactly matching the sum of the two step values, confirming that ΔG° (like ΔH°) is additive along any reaction pathway, exactly as Hess's Law established for ΔH° in Unit II.

**Appendix Problem A6 — Putting it all together: a multi-part phase-equilibrium problem** Naphthalene has a normal sublimation pressure of 1.00 mmHg at 325 K and a normal melting point of 353 K with ΔHfus = 19.0 kJ mol⁻¹. Its ΔHsub (solid → vapour) is 73.0 kJ mol⁻¹, essentially constant below the melting point.

3. Estimate the sublimation pressure of solid naphthalene at 340 K.

4. Using ΔHsub = ΔHfus + ΔHvap (Hess's-Law-type additivity of enthalpies for the two-step path solid→liquid→vapour, compared with the one-step path solid→vapour), estimate ΔHvap for naphthalene.

Solution:

(1) log(P2/1.00) = [73 000/(2.303×8.314)] × [(340−325)/(325×340)] = 3812.6 × (15/110 500) = 0.5175 P2 = 10^0.5175 ≈ 3.29 mmHg — a substantial rise in sublimation pressure over just 15 K, again illustrating the strong (exponential) temperature sensitivity typical of the Clausius–Clapeyron relation.

(2) ΔHvap = ΔHsub − ΔHfus = 73.0 − 19.0 = 54.0 kJ mol⁻¹ — a value consistent with typical vaporisation enthalpies for molecules of comparable size and polarity, and a useful cross-check whenever both sublimation and fusion data are available for the same substance.

#### Appendix Problem A7 — Free-energy and entropy criteria applied together
{: .example}

A reaction has ΔH° = −65.0 kJ mol⁻¹ and ΔS° = −120 J K⁻¹ mol⁻¹ at 298 K. (a) Calculate ΔG° and state whether the reaction is spontaneous at 298 K. (b) Find the temperature above which the reaction ceases to be spontaneous. (c) Comment on how this behaviour is consistent with Le Chatelier-type reasoning that an exothermic reaction is favoured by lowering the temperature.

Solution:

(a) ΔG° = ΔH° − TΔS° = −65 000 − 298(−120) = −65 000 + 35 760 = −29 240 J ≈ −29.2 kJ; since ΔG° < 0, the reaction is spontaneous at 298 K.

(b) The reaction ceases to be spontaneous once ΔG° = 0, i.e. at T = ΔH°/ΔS° = (−65 000)/(−120) = 541.7 K; above this temperature ΔG° becomes positive.

(c) This is entirely consistent with the qualitative rule that lowering temperature favours an exothermic reaction: because ΔS° is negative here, the −TΔS° term becomes less unfavourable (smaller and positive) as T is lowered, reinforcing the already-favourable (negative) ΔH° term, so the reaction remains spontaneous at low T and only becomes non-spontaneous once T is raised past 541.7 K — precisely the pattern given generally in the sign-combination table of Section 3.3.

## Summary of Key Equations — Unit III

|**Topic**|**Key equation(s)**|
|---|---|
|Helmholtz energy|A = E − TS;−ΔA = wrev(max)|
|Gibbs energy|G = H − TS;−ΔG = net(non-expansion)work|
|Spontaneity (T, P constant)|dG < 0 spontaneous; dG = 0 equilibrium|
|Gibbs–Helmholtz(G, H)|ΔG = ΔH + T[∂(ΔG)/∂T]P|
|Gibbs–Helmholtz(A, E)|ΔA = ΔE + T[∂(ΔA)/∂T]V|
|Standard Gibbs energyof reaction|ΔG° = ΣΔGf°(products)− ΣΔGf°(reactants)= ΔH° − TΔS°|
|T, P dependence of G|(∂G/∂T)P = −S; (∂G/∂P)T = V|
|ΔG,isothermal(idealgas)|ΔG = nRT ln(P2/P1)|
|Clapeyron equation|dP/dT = ΔH /[T(V2−V1)]|
|Clausius–Clapeyron(integrated)|log(P2/P1)=[ΔH/2.303R][(T2−T1)/(T1T2)]|
|Partial molarproperty|X̄i =(∂X/∂ni)T,P,nj;  X = Σ ni X̄i|
|Gibbs–Duhem equation|Σ ni dμi = 0(constant T,P)|
|Chemicalpotential|μi =(∂G/∂ni)T,P,nj|
|μvs T,P|(∂μi/∂T)P = −S̄i;(∂μi/∂P)T = V̄i|
|Maxwell's relations|(∂S/∂V)T=(∂P/∂T)V;  (∂S/∂P)T=−(∂V/∂T)P; and two more (see Section<br>10.4)|

## Review Questions

#### A. Short-Answer Questions (Remember / Understand)

1. Define the Helmholtz free energy and the Gibbs free energy.

2. State the criteria for spontaneity and equilibrium in terms of dG at constant temperature and pressure.

3. Define the standard Gibbs energy of formation. What is its value for an element in its standard state?

4. Write the two partial derivatives giving the temperature and pressure dependence of G.

5. State the Clapeyron equation and identify each term in it.

6. What approximations convert the Clapeyron equation into the Clausius–Clapeyron equation?

7. Define a partial molar property, giving its mathematical definition.

8. State the Gibbs–Duhem equation and explain, in one sentence, its physical meaning.

9. Define chemical potential. Why is it sometimes called an 'escaping tendency'?

10. Write the four fundamental (combined-law) thermodynamic equations from which Maxwell's relations are derived.

#### B. Long-Answer / Derivation Questions (Apply / Analyze)

11. Derive the Gibbs–Helmholtz equation relating ΔG, ΔH and the temperature coefficient of ΔG.

12. Derive the Clapeyron equation for the equilibrium between two phases of a pure substance.

13. Starting from the Clapeyron equation, derive the integrated form of the Clausius–Clapeyron equation, stating clearly the assumptions involved.

14. Derive the Gibbs–Duhem equation, starting from the expression G = Σ ni μi.

15. Derive the variation of chemical potential with temperature and with pressure.

16. Derive all four Maxwell relations from the four fundamental thermodynamic equations, showing the reciprocity condition used in each case.

17. Show that (∂S/∂V)T for an ideal gas, obtained from a Maxwell relation, is consistent with the ideal-gas entropy expression derived from the First and Second Laws directly.

#### C. Numerical Problems (Apply / Analyze / Evaluate)

18. For a reaction at 298 K, ΔH = −50.0 kJ mol⁻¹ and ΔG = −42.0 kJ mol⁻¹. Estimate ΔG at 320 K, assuming (∂ΔG/∂T)P remains constant.

19. Using standard Gibbs energies of formation, calculate ΔG° for the reaction CH4(g) + 2O2(g) → CO2(g) + 2H2O(l), given ΔGf°: CH4 −50.8, CO2 −394.4, H2O(l) −237.1 kJ mol⁻¹ (O2 = 0).

20. 3 mol of an ideal gas expand isothermally and reversibly from 2 L to 20 L at 350 K. Calculate ΔG for the process.

21. The vapour pressure of a liquid is 100 mmHg at 320 K and 400 mmHg at 350 K. Calculate the molar heat of vaporisation.

22. Estimate the boiling point of a liquid at 720 mmHg, given that it boils at 350 K under 760 mmHg and has ΔHvap = 32 kJ mol⁻¹.

23. Calculate the molal elevation constant of a solvent whose boiling point is 350 K and whose latent heat of vaporisation is 400 cal g⁻¹.

24. In a binary solution with n1 = 3 mol and n2 = 5 mol, μ1 changes by +300 J mol⁻¹ over a small composition range. Use the Gibbs–Duhem equation to find the corresponding change in μ2.

25. Estimate the change in chemical potential of an ideal gas at 310 K when its pressure changes from 2 atm to 8 atm.

26. For a metal with Cp = 25 J K⁻¹ mol⁻¹ between 250 K and 300 K, outline (qualitatively) how the Maxwell relation (∂S/∂P)T = −(∂V/∂T)P could be combined with heat-capacity data to estimate the entropy change of the metal when both its temperature and pressure change.

#### D. Higher-Order Thinking (HOTS) Questions (Evaluate / Create)

_The following questions require integration of more than one concept from this unit and are of JAM/competitive-examination difficulty._

27. Using the Gibbs–Helmholtz equation, show how a plot of ΔG/T against 1/T can be used to obtain ΔH for a reaction directly from its slope, and discuss the advantage of this graphical method over using just two temperatures.

28. A liquid shows an unusually flat Clausius–Clapeyron plot (log P vs 1/T) over a wide temperature range near its critical point. Explain, in terms of the assumptions underlying the Clausius–Clapeyron equation, why the equation becomes progressively less reliable as the critical point is approached.

29. Using the Gibbs–Duhem equation, explain why it is thermodynamically impossible for the activity coefficients of both components of a binary solution to increase simultaneously with increasing mole fraction of one component, over the same composition range.

30. Combine the chemical-potential equilibrium condition (μ same in every phase) with the Clapeyron equation to explain, in your own words, why the boiling point of a liquid must always increase with increasing external pressure, whereas the melting point of ice is unusual in decreasing with increasing pressure.

31. Derive, using Maxwell's relations, an expression for (∂Cp/∂P)T in terms of (∂²V/∂T²)P, and comment on why this quantity is generally very small for an ideal gas but can be significant for a real gas or liquid near a phase transition.

## Quick Revision Checklist

Use this checklist for last-minute revision before a test on this unit. Tick off each item once you can state it, derive it, or solve a numerical based on it without referring to notes.

- Definitions of A and G, and the maximum-work interpretation of −ΔA and −ΔG.

- The five spontaneity/equilibrium criteria (constant E,V; S,V; S,P; T,V; T,P).

- Full derivation of the Gibbs–Helmholtz equation, ΔG = ΔH + T(∂ΔG/∂T)P.

- Calculation of ΔG° of a reaction from tabulated ΔGf° values, and from ΔH° and ΔS°.

- (∂G/∂T)P = −S and (∂G/∂P)T = V, and the isothermal ΔG expression for an ideal gas.

- Full derivation of the Clapeyron equation, dP/dT = ΔH/[T(V2−V1)].

- Derivation of the Clausius–Clapeyron equation from the Clapeyron equation, and its four standard applications.

- Definition of a partial molar property and the additivity relation X = Σ ni X̄i.

- Derivation and physical meaning of the Gibbs–Duhem equation, Σ ni dμi = 0.

- Definition of chemical potential, its escaping-tendency interpretation, and its variation with T and P.

- The four fundamental thermodynamic equations and the derivation of all four Maxwell relations from them.

- At least one worked application of a Maxwell relation to connect entropy with measurable P– V–T data.

---

[← Course home](./) · [Back to top](#)
{% endraw %}
