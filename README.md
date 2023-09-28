<html>

<h1>
<span style='font-size:30pt;font-family:"Open Sans"'>ESE-EE-DNN &ndash; Easy
Solvation Energy Evaluation with Electronegativity Equalization and Dense Neural Network</span></h1>

<h2><span style='font-family:"Open Sans"'>Introduction and User's Guide</span></h2>

<p style='margin-top:12pt'><span style='font-family:"Open Sans"'>
<i>ESE-EE-DNN</i> is a method for evaluation of <b>solvation free energies</b> of molecules 
and ions [2]. It requires the solute molecular geometry and the total charge only.
To obtain the solvation free energy, first <i>electronegativity-equalization</i>
atomic charges are calculated. Subsequently, the solute van der Waals surface is constructed,
and induced surface charges and the COSMO electrostatic energy are computed.
The results, as well as three solvent features are fed into a <i>Dense Neural Network</i>
that eventually yields the solvation free energy.</span></p>

<p style='margin-top:12pt'><span style='font-family:"Open Sans"'>
<i>ESE-EE-DNN</i> is an improved machine-learning adaptation of my <i>ESE-EE</i> scheme [3],
which is in turn based on the <a href="https://github.com/vyboishchikov/ESE">uESE</a> [3] and xESE [4]
that we developed jointly with Alexander Voityuk.</span></p>

<p style='margin-top:12pt'><span style='font-family:"Open Sans"'>
The supported elements are H, C, N, O, F, Si, P, S, Cl, Br, I.</p>

<p style='margin-top:12pt;margin-bottom:0cm'><span style='font-family:"Open Sans"'>
The ESE-EE-DNN solvation free energy can be calculated by the program ESE-EE-DNN,
which can be downloaded here free of charge:</span></p>

<p style='margin:0cm;margin-bottom:0pt'><span style='font-family:"Open Sans"'>
<a href="https://github.com/vyboishchikov/ESE-EE-DNN/blob/main/ESE-EE-DNN.exe">ESE-EE-DNN.exe</a> &ndash; Windows version</span></p>

<p style='margin:0cm;margin-bottom:0pt'><span style='font-family:"Open Sans"'>
<a href="https://github.com/vyboishchikov/ESE-EE-DNN/blob/main/ESE-EE-DNN.x">ESE-EE-DNN.x</a> &ndash; Linux version</span></p>

</p>

<p style='margin:0cm;margin-bottom:0pt'><span style='font-family:"Open Sans"'>
The ESE-EE-DNN program can be run from the command line as follows:</span></p>

<p style='margin-top:6pt;margin-right:0cm;margin-bottom:0cm;margin-left:0cm'>
<tt><b>ESE-EE-DNN.exe <i>xyz-file</i> -charge <i>charge</i> -solvent <i>solvent</i></b></tt></p>

<p style='margin-top:12pt;margin-bottom:0pt'><span style='font-family:"Open Sans"'>
If your solvent is not in this <a href="https://github.com/vyboishchikov/ESE-EE-DNN/blob/main/solvent-list.html">list</a>, you can use the following call format:</span></p>

<p style='margin-top:6pt;margin-bottom:12pt'><tt><b>ESE-EE-DNN.exe <i>xyz-file</i> -charge <i>
charge</i> -Eps <i>dielectric_constant</i> -BP <i>boiling_point_&deg;C</i> -Nheavy <i> number_of_non_hydrogen_atoms_in_solvent</i></b>
</tt></p>

<p style='margin:0cm'><span style='font-family:"Open Sans"'>
Once you use results calculated by the ESE-EE-DNN program, you should include at least the
following citations: </span></p>

<p style='margin:0cm'><span style='font-family:"Open Sans"'>
<b>1</b>. S. F. Vyboishchikov, <i>ESE-EE-DNN program</i>, Girona, <b>2023</b></span></p>

<p style='margin:0cm;margin-bottom:12pt'><span style='font-family:"Open Sans"'>
<b>2</b>. S. F. Vyboishchikov, <i>J. Chem. Inf. Model</i>.,<b>2023</b>, <i>63</i>, <i>in press</i>.
<a href="https://doi.org/10.1021/acs.jcim.3c00922">DOI: 10.1021/acs.jcim.3c00922</a></span></p>

<p style='margin-bottom:0pt'><span style='font-family:"Open Sans"'>
and preferably also cite our previous related work:</span></p>

<p style='margin:0cm;margin-bottom:0pt'><span style='font-family:"Open Sans"'>
<b>3</b>. S. F. Vyboishchikov, <i>J. Comput. Chem.</i>, <b>2023</b>, <i>44</i>, 307&ndash;318. 
<a href="https://doi.org/10.1002/jcc.26894">DOI: 10.1002/jcc.26894</a></span></p>

<p style='margin:0cm;margin-bottom:0pt'><span style='font-family: "Open Sans"'>
<b>4</b>. S. F. Vyboishchikov, A. A. Voityuk, <i> Chemical Reactivity, vol. 2:
Approaches and applications, S. Kaya, L. von Szentp&aacute;ly, G. Serdaro&gbreve;lu, K. Guo (Eds.)</i>,
Elsevier, Amsterdam, <b>2023</b>, 399&ndash;427. <a href="https://doi.org/10.1016/B978-0-32-390259-5.00021-4">
DOI: 10.1016/B978-0-32-390259-5.00021-4</a></span></p>

<p style='margin:0cm;margin-bottom:0pt'><span style='font-family:"Open Sans"'>
<b>5</b>. S. F. Vyboishchikov, A. A. Voityuk, <a href="https://pubs.acs.org/doi/10.1021/acs.jcim.1c00885">
<i>J. Chem. Inf. Model., </i><b>2021</b>, <i>61</i></a>, 4544&ndash;4553. DOI: 10.1021/acs.jcim.1c00885 </span></p>

<p style='margin:0cm;margin-bottom:0pt'><span style='font-family:"Open Sans"'>
<b>6</b>. S. F. Vyboishchikov, A. A. Voityuk, <a href="https://onlinelibrary.wiley.com/doi/abs/10.1002/jcc.26531">
<i>J. Comput. Chem., </i><b>2021</b>, <i>42</i></a>, 1184&ndash;1194. DOI: 10.1002/jcc.26531</span></p>

<p style='margin:0cm;margin-bottom:0pt'><span style='font-family: "Open Sans"'>
<b>7</b>. A. A. Voityuk, S. F. Vyboishchikov, <a href="https://pubs.rsc.org/en/content/articlelanding/2020/cp/d0cp02667k">
<i>Phys. Chem. Chem. Phys.</i> <b>2020</b>, <i>22</i></a>, 14591&ndash;14598. DOI: 10.1039/d0cp02667k</span></p>

<p style='margin:0cm;margin-bottom:0pt'><span style='font-family: "Open Sans"'>
<b>8</b>. A. A. Voityuk, S. F. Vyboishchikov, <a href="https://pubs.rsc.org/en/content/articlelanding/2019/cp/c9cp03010g">
<i>Phys. Chem. Chem. Phys.</i>, <b>2019</b>, <i>21</i></a>, 875&ndash;874. DOI: 10.1039/c9cp03010g</span></p>

<p style='margin:0cm;margin-top:12pt'><span style='font-family: "Open Sans"'>
Questions related to the ESE-EE-DNN method and program should be addressed to
<a href="mailto:vyboishchikov@googlemail.com">Sergei Vyboishchikov</a>.</p>

</html>
