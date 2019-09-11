"# PHP-aula4-ex4" 
<?xml version="1.0" encoding="utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" lang="en" xml:lang="en">
<head>
<!-- 2019-09-10 ter 22:02 -->
<meta http-equiv="Content-Type" content="text/html;charset=utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>&lrm;</title>
<meta name="generator" content="Org mode" />
<style type="text/css">
 <!--/*--><![CDATA[/*><!--*/
  .title  { text-align: center;
             margin-bottom: .2em; }
  .subtitle { text-align: center;
              font-size: medium;
              font-weight: bold;
              margin-top:0; }
  .todo   { font-family: monospace; color: red; }
  .done   { font-family: monospace; color: green; }
  .priority { font-family: monospace; color: orange; }
  .tag    { background-color: #eee; font-family: monospace;
            padding: 2px; font-size: 80%; font-weight: normal; }
  .timestamp { color: #bebebe; }
  .timestamp-kwd { color: #5f9ea0; }
  .org-right  { margin-left: auto; margin-right: 0px;  text-align: right; }
  .org-left   { margin-left: 0px;  margin-right: auto; text-align: left; }
  .org-center { margin-left: auto; margin-right: auto; text-align: center; }
  .underline { text-decoration: underline; }
  #postamble p, #preamble p { font-size: 90%; margin: .2em; }
  p.verse { margin-left: 3%; }
  pre {
    border: 1px solid #ccc;
    box-shadow: 3px 3px 3px #eee;
    padding: 8pt;
    font-family: monospace;
    overflow: auto;
    margin: 1.2em;
  }
  pre.src {
    position: relative;
    overflow: visible;
    padding-top: 1.2em;
  }
  pre.src:before {
    display: none;
    position: absolute;
    background-color: white;
    top: -10px;
    right: 10px;
    padding: 3px;
    border: 1px solid black;
  }
  pre.src:hover:before { display: inline;}
  /* Languages per Org manual */
  pre.src-asymptote:before { content: 'Asymptote'; }
  pre.src-awk:before { content: 'Awk'; }
  pre.src-C:before { content: 'C'; }
  /* pre.src-C++ doesn't work in CSS */
  pre.src-clojure:before { content: 'Clojure'; }
  pre.src-css:before { content: 'CSS'; }
  pre.src-D:before { content: 'D'; }
  pre.src-ditaa:before { content: 'ditaa'; }
  pre.src-dot:before { content: 'Graphviz'; }
  pre.src-calc:before { content: 'Emacs Calc'; }
  pre.src-emacs-lisp:before { content: 'Emacs Lisp'; }
  pre.src-fortran:before { content: 'Fortran'; }
  pre.src-gnuplot:before { content: 'gnuplot'; }
  pre.src-haskell:before { content: 'Haskell'; }
  pre.src-hledger:before { content: 'hledger'; }
  pre.src-java:before { content: 'Java'; }
  pre.src-js:before { content: 'Javascript'; }
  pre.src-latex:before { content: 'LaTeX'; }
  pre.src-ledger:before { content: 'Ledger'; }
  pre.src-lisp:before { content: 'Lisp'; }
  pre.src-lilypond:before { content: 'Lilypond'; }
  pre.src-lua:before { content: 'Lua'; }
  pre.src-matlab:before { content: 'MATLAB'; }
  pre.src-mscgen:before { content: 'Mscgen'; }
  pre.src-ocaml:before { content: 'Objective Caml'; }
  pre.src-octave:before { content: 'Octave'; }
  pre.src-org:before { content: 'Org mode'; }
  pre.src-oz:before { content: 'OZ'; }
  pre.src-plantuml:before { content: 'Plantuml'; }
  pre.src-processing:before { content: 'Processing.js'; }
  pre.src-python:before { content: 'Python'; }
  pre.src-R:before { content: 'R'; }
  pre.src-ruby:before { content: 'Ruby'; }
  pre.src-sass:before { content: 'Sass'; }
  pre.src-scheme:before { content: 'Scheme'; }
  pre.src-screen:before { content: 'Gnu Screen'; }
  pre.src-sed:before { content: 'Sed'; }
  pre.src-sh:before { content: 'shell'; }
  pre.src-sql:before { content: 'SQL'; }
  pre.src-sqlite:before { content: 'SQLite'; }
  /* additional languages in org.el's org-babel-load-languages alist */
  pre.src-forth:before { content: 'Forth'; }
  pre.src-io:before { content: 'IO'; }
  pre.src-J:before { content: 'J'; }
  pre.src-makefile:before { content: 'Makefile'; }
  pre.src-maxima:before { content: 'Maxima'; }
  pre.src-perl:before { content: 'Perl'; }
  pre.src-picolisp:before { content: 'Pico Lisp'; }
  pre.src-scala:before { content: 'Scala'; }
  pre.src-shell:before { content: 'Shell Script'; }
  pre.src-ebnf2ps:before { content: 'ebfn2ps'; }
  /* additional language identifiers per "defun org-babel-execute"
       in ob-*.el */
  pre.src-cpp:before  { content: 'C++'; }
  pre.src-abc:before  { content: 'ABC'; }
  pre.src-coq:before  { content: 'Coq'; }
  pre.src-groovy:before  { content: 'Groovy'; }
  /* additional language identifiers from org-babel-shell-names in
     ob-shell.el: ob-shell is the only babel language using a lambda to put
     the execution function name together. */
  pre.src-bash:before  { content: 'bash'; }
  pre.src-csh:before  { content: 'csh'; }
  pre.src-ash:before  { content: 'ash'; }
  pre.src-dash:before  { content: 'dash'; }
  pre.src-ksh:before  { content: 'ksh'; }
  pre.src-mksh:before  { content: 'mksh'; }
  pre.src-posh:before  { content: 'posh'; }
  /* Additional Emacs modes also supported by the LaTeX listings package */
  pre.src-ada:before { content: 'Ada'; }
  pre.src-asm:before { content: 'Assembler'; }
  pre.src-caml:before { content: 'Caml'; }
  pre.src-delphi:before { content: 'Delphi'; }
  pre.src-html:before { content: 'HTML'; }
  pre.src-idl:before { content: 'IDL'; }
  pre.src-mercury:before { content: 'Mercury'; }
  pre.src-metapost:before { content: 'MetaPost'; }
  pre.src-modula-2:before { content: 'Modula-2'; }
  pre.src-pascal:before { content: 'Pascal'; }
  pre.src-ps:before { content: 'PostScript'; }
  pre.src-prolog:before { content: 'Prolog'; }
  pre.src-simula:before { content: 'Simula'; }
  pre.src-tcl:before { content: 'tcl'; }
  pre.src-tex:before { content: 'TeX'; }
  pre.src-plain-tex:before { content: 'Plain TeX'; }
  pre.src-verilog:before { content: 'Verilog'; }
  pre.src-vhdl:before { content: 'VHDL'; }
  pre.src-xml:before { content: 'XML'; }
  pre.src-nxml:before { content: 'XML'; }
  /* add a generic configuration mode; LaTeX export needs an additional
     (add-to-list 'org-latex-listings-langs '(conf " ")) in .emacs */
  pre.src-conf:before { content: 'Configuration File'; }

  table { border-collapse:collapse; }
  caption.t-above { caption-side: top; }
  caption.t-bottom { caption-side: bottom; }
  td, th { vertical-align:top;  }
  th.org-right  { text-align: center;  }
  th.org-left   { text-align: center;   }
  th.org-center { text-align: center; }
  td.org-right  { text-align: right;  }
  td.org-left   { text-align: left;   }
  td.org-center { text-align: center; }
  dt { font-weight: bold; }
  .footpara { display: inline; }
  .footdef  { margin-bottom: 1em; }
  .figure { padding: 1em; }
  .figure p { text-align: center; }
  .inlinetask {
    padding: 10px;
    border: 2px solid gray;
    margin: 10px;
    background: #ffffcc;
  }
  #org-div-home-and-up
   { text-align: right; font-size: 70%; white-space: nowrap; }
  textarea { overflow-x: auto; }
  .linenr { font-size: smaller }
  .code-highlighted { background-color: #ffff00; }
  .org-info-js_info-navigation { border-style: none; }
  #org-info-js_console-label
    { font-size: 10px; font-weight: bold; white-space: nowrap; }
  .org-info-js_search-highlight
    { background-color: #ffff00; color: #000000; font-weight: bold; }
  .org-svg { width: 90%; }
  /*]]>*/-->
</style>
<script type="text/javascript">
/*
@licstart  The following is the entire license notice for the
JavaScript code in this tag.

Copyright (C) 2012-2019 Free Software Foundation, Inc.

The JavaScript code in this tag is free software: you can
redistribute it and/or modify it under the terms of the GNU
General Public License (GNU GPL) as published by the Free Software
Foundation, either version 3 of the License, or (at your option)
any later version.  The code is distributed WITHOUT ANY WARRANTY;
without even the implied warranty of MERCHANTABILITY or FITNESS
FOR A PARTICULAR PURPOSE.  See the GNU GPL for more details.

As additional permission under GNU GPL version 3 section 7, you
may distribute non-source (e.g., minimized or compacted) forms of
that code without the copy of the GNU GPL normally required by
section 4, provided you include this license notice and a URL
through which recipients can access the Corresponding Source.


@licend  The above is the entire license notice
for the JavaScript code in this tag.
*/
<!--/*--><![CDATA[/*><!--*/
 function CodeHighlightOn(elem, id)
 {
   var target = document.getElementById(id);
   if(null != target) {
     elem.cacheClassElem = elem.className;
     elem.cacheClassTarget = target.className;
     target.className = "code-highlighted";
     elem.className   = "code-highlighted";
   }
 }
 function CodeHighlightOff(elem, id)
 {
   var target = document.getElementById(id);
   if(elem.cacheClassElem)
     elem.className = elem.cacheClassElem;
   if(elem.cacheClassTarget)
     target.className = elem.cacheClassTarget;
 }
/*]]>*///-->
</script>
</head>
<body>
<div id="content">
<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#org7d29bda">1. SESSÕES</a>
<ul>
<li><a href="#org8b1cd22">1.1. Exercício 1</a></li>
<li><a href="#org0ff77f9">1.2. Site de perguntas</a></li>
<li><a href="#org9b9cf16">1.3. SESSION</a></li>
<li><a href="#org44524af">1.4. Iniciando a sessão</a></li>
<li><a href="#org22148d3">1.5. Modificar um valor</a></li>
<li><a href="#org82e6b38">1.6. Terminar uma sessão</a></li>
<li><a href="#orgebdf379">1.7. Exercício 2</a></li>
<li><a href="#orgf222e42">1.8. Exercício 3</a></li>
<li><a href="#orgf23b787">1.9. Exercício 4</a></li>
</ul>
</li>
</ul>
</div>
</div>

<div id="outline-container-org7d29bda" class="outline-2">
<h2 id="org7d29bda"><span class="section-number-2">1</span> SESSÕES</h2>
<div class="outline-text-2" id="text-1">
<p>
Com sessões você pode armazenar informações em variáveis e utilizar em várias páginas diferentes.
</p>

<p>
A informação é armazenada no servidor e não no computador local.
</p>
</div>

<div id="outline-container-org8b1cd22" class="outline-3">
<h3 id="org8b1cd22"><span class="section-number-3">1.1</span> Exercício 1</h3>
<div class="outline-text-3" id="text-1-1">
<p>
Crie 4 páginas com perguntas para o usuário, quando o usuário acertar a pergunta mostre a próxima pergunta em outra página e exiba a quantidade de acertos e erros:
</p>

<pre class="example">
Perguntas: 3
Certas: 2
Erradas: 1
</pre>

<p>
Utilize um input escondido (<code>type="hidden"</code>) para transportar os valores para outra página.
</p>
</div>
</div>

<div id="outline-container-org0ff77f9" class="outline-3">
<h3 id="org0ff77f9"><span class="section-number-3">1.2</span> Site de perguntas</h3>
<div class="outline-text-3" id="text-1-2">
<p>
Implemente um website de perguntas e respostas utilizando PHP, a página deve passar a resposta atual, a quantidade de acertos e erros para a próxima página nas linhas 13 e 14.
</p>

<pre class="example">
<span class="linenr"> 1: </span>&lt;!DOCTYPE html&gt;
<span class="linenr"> 2: </span>&lt;html lang="en"&gt;
<span class="linenr"> 3: </span>&lt;head&gt;
<span class="linenr"> 4: </span>    &lt;meta charset="UTF-8"&gt;
<span class="linenr"> 5: </span>    &lt;title&gt;Questão 1&lt;/title&gt;
<span class="linenr"> 6: </span>&lt;/head&gt;
<span class="linenr"> 7: </span>&lt;body&gt;
<span class="linenr"> 8: </span>   &lt;h1&gt;text-align&lt;/h1&gt;
<span class="linenr"> 9: </span>   &lt;p&gt;Em CSS, as opções de valores para text-align são: center, left, right e justify&lt;/p&gt;
<span class="linenr">10: </span>    &lt;form action="dois.php"&gt;
<span class="linenr">11: </span>        &lt;input type="radio" name="resposta" value="sim"&gt;Sim &lt;br&gt;
<span class="linenr">12: </span>        &lt;input type="radio" name="resposta" value="nao"&gt;Não &lt;br&gt;
<span class="linenr">13: </span>        &lt;input type="hidden" name="acertos" value="0"&gt;
<span class="linenr">14: </span>        &lt;input type="hidden" name="erros" value="0"&gt;
<span class="linenr">15: </span>        &lt;input type="submit" value="Responder"&gt;
<span class="linenr">16: </span>    &lt;/form&gt;
<span class="linenr">17: </span>&lt;/body&gt;
<span class="linenr">18: </span>&lt;/html&gt;
</pre>

<p>
No código acima, os dois campos com <code>type="hidden"</code> guardam os valores atuais de acertos e erros, esses valores são transferidos para a próxima página quando o usuário aperta o botão <b>Responder</b>.
</p>

<p>
No código abaixo, verificamos a resposta, se for correta aumentamos o valor de $acertos se for incorreta aumentamos o valor de $erros, linhas 11 à 17. Continuamos enviando as quantidades de acertos e erros usando os campos input. Os values desses campos são atualizados utilizando o PHP nas linhas 25 e 26. Além de imprimir uma tabela com os acertos e erros, linhas 35 e 38.
</p>

<pre class="example">
<span class="linenr"> 1: </span>&lt;!DOCTYPE html&gt;
<span class="linenr"> 2: </span>&lt;html lang="en"&gt;
<span class="linenr"> 3: </span>&lt;head&gt;
<span class="linenr"> 4: </span>    &lt;meta charset="UTF-8"&gt;
<span class="linenr"> 5: </span>    &lt;title&gt;Questão 1&lt;/title&gt;
<span class="linenr"> 6: </span>&lt;/head&gt;
<span class="linenr"> 7: </span>&lt;body&gt;
<span class="linenr"> 8: </span>&lt;?php
<span class="linenr"> 9: </span>    $resposta = $_GET['resposta'];
<span class="linenr">10: </span>    
<span class="linenr">11: </span>    if($resposta == 'nao') {
<span class="linenr">12: </span>        $acertos = $_GET['acertos'] + 1;
<span class="linenr">13: </span>        $erros = $_GET['erros'];
<span class="linenr">14: </span>    } else {
<span class="linenr">15: </span>        $acertos = $_GET['acertos'];
<span class="linenr">16: </span>        $erros = $_GET['erros'] + 1;
<span class="linenr">17: </span>    }
<span class="linenr">18: </span>?&gt;
<span class="linenr">19: </span>   &lt;h1&gt;text-align&lt;/h1&gt;
<span class="linenr">20: </span>   &lt;p&gt;Em CSS, as opções de valores para text-align são: center, left, right e justify&lt;/p&gt;
<span class="linenr">21: </span>    &lt;form action="dois.php"&gt;
<span class="linenr">22: </span>        &lt;input type="radio" name="resposta" value="sim"&gt;Sim &lt;br&gt;
<span class="linenr">23: </span>        &lt;input type="radio" name="resposta" value="nao"&gt;Não &lt;br&gt;
<span class="linenr">24: </span>&lt;?php
<span class="linenr">25: </span>    echo "&lt;input type='hidden' name='acertos' value='$acertos'&gt;\n";
<span class="linenr">26: </span>    echo "&lt;input type='hidden' name='erros' value='$erros'&gt;";  
<span class="linenr">27: </span>?&gt;
<span class="linenr">28: </span>        &lt;input type="submit" value="Responder"&gt;
<span class="linenr">29: </span>    &lt;/form&gt;
<span class="linenr">30: </span>    &lt;br&gt;
<span class="linenr">31: </span>    &lt;table border="1"&gt;
<span class="linenr">32: </span>        &lt;tr&gt;&lt;th&gt;Acertos&lt;/th&gt;&lt;th&gt;Erros&lt;/th&gt;&lt;/tr&gt;
<span class="linenr">33: </span>        &lt;tr&gt;
<span class="linenr">34: </span>            &lt;td&gt;
<span class="linenr">35: </span>                &lt;?php echo $acertos; ?&gt;
<span class="linenr">36: </span>            &lt;/td&gt;
<span class="linenr">37: </span>            &lt;td&gt;
<span class="linenr">38: </span>                &lt;?php echo $erros; ?&gt;
<span class="linenr">39: </span>            &lt;/td&gt;
<span class="linenr">40: </span>        &lt;/tr&gt;
<span class="linenr">41: </span>    &lt;/table&gt;
<span class="linenr">42: </span>&lt;/body&gt;
<span class="linenr">43: </span>&lt;/html&gt;
</pre>
</div>
</div>

<div id="outline-container-org9b9cf16" class="outline-3">
<h3 id="org9b9cf16"><span class="section-number-3">1.3</span> SESSION</h3>
<div class="outline-text-3" id="text-1-3">
<p>
O protocolo HTTP utilizado na internet não guarda o estado do usuário.
</p>

<p>
Ao fechar um website e abrir novamente você acessa uma nova cópia. 
</p>

<p>
Ao acessar outra página do mesmo website normalmente nenhuma informação sobre o usuário é mantida.
</p>

<p>
Variáveis de sessão armazenam informações que podem ser usadas em várias páginas, resolvendo o problema.
</p>
</div>
</div>

<div id="outline-container-org44524af" class="outline-3">
<h3 id="org44524af"><span class="section-number-3">1.4</span> Iniciando a sessão</h3>
<div class="outline-text-3" id="text-1-4">
<p>
Para utilizar sessão é necessário executar a função <b>session_start()</b>.
</p>

<p>
As variáveis são armazenadas em <b>$_SESSION</b>.
</p>

<pre class="example">
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;body&gt;

&lt;?php
// inicia sessão nesta página
session_start();

// armazena o valor de corfavorita
$_SESSION["corfavorita"] = "verde";

echo "Valor armazenado!";
?&gt;

&lt;a href="segunda.php"&gt;Próxima&lt;/a&gt;
&lt;/body&gt;
&lt;/html&gt;
</pre>

<p>
Podemos usar o valor em outra página:
</p>

<pre class="example">
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;body&gt;

&lt;?php
// inicia sessão nesta página
session_start();

echo $_SESSION["corfavorita"];
?&gt;
&lt;a href="terceira.php"&gt;Próxima&lt;/a&gt;
&lt;/body&gt;
&lt;/html&gt;
</pre>

<p>
A função <b>session_start()</b> deve ser executada toda vez que quiser utilizar (armazenar ou usar) os valores em $_SESSION.
</p>
</div>
</div>

<div id="outline-container-org22148d3" class="outline-3">
<h3 id="org22148d3"><span class="section-number-3">1.5</span> Modificar um valor</h3>
<div class="outline-text-3" id="text-1-5">
<p>
Para alterar um valor em $_SESSION, basta atribuir um novo valor:
</p>

<pre class="example">
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;body&gt;

&lt;?php
// inicia sessão nesta página
session_start();

// armazena o valor de corfavorita
$_SESSION["corfavorita"] = "azul";

echo "Valor trocado!";
?&gt;

&lt;a href="quarta.php"&gt;Finalizar&lt;/a&gt;
&lt;/body&gt;
&lt;/html&gt;
</pre>
</div>
</div>

<div id="outline-container-org82e6b38" class="outline-3">
<h3 id="org82e6b38"><span class="section-number-3">1.6</span> Terminar uma sessão</h3>
<div class="outline-text-3" id="text-1-6">
<p>
Para terminar uma sessão usamos as funções <b>session_unset()</b> e <b>session_destroy()</b>:
</p>

<pre class="example">
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;body&gt;

&lt;?php
// inicia sessão nesta página
session_start();

// remover todas as variáveis
session_unset();

// destruir a sessão
session_destroy();

echo "Sessão encerrada!";
?&gt;

&lt;/body&gt;
&lt;/html&gt;
</pre>
</div>
</div>


<div id="outline-container-orgebdf379" class="outline-3">
<h3 id="orgebdf379"><span class="section-number-3">1.7</span> Exercício 2</h3>
<div class="outline-text-3" id="text-1-7">
<p>
Implemente o exercício 1 utilizando sessões.
</p>

<pre class="example">
Perguntas: 3
Certas: 2
Erradas: 1
</pre>

<p>
Utilize uma variável em $_SESSION para transportar os valores para outra página.
</p>
</div>
</div>

<div id="outline-container-orgf222e42" class="outline-3">
<h3 id="orgf222e42"><span class="section-number-3">1.8</span> Exercício 3</h3>
<div class="outline-text-3" id="text-1-8">
<p>
Crie uma página que recebe a cor favorita de um usuário usando:
</p>

<pre class="example">
&lt;input type="color" name="cor"&gt;
</pre>

<p>
Armazene a cor escolhida em:
</p>

<pre class="example">
$_SESSION['corescolhida'] = $_GET['cor'];
</pre>

<p>
Em seguida use a cor selecionada como cor de fundo nas páginas do exercício anterior utilizando sessão, exemplo:
</p>

<pre class="example">
&lt;style&gt;
   body {
      color: &lt;?php 
         session_start();
         echo $_SESSION['corescolhida']; 
      ?&gt;
   }
&lt;/style&gt;
</pre>
</div>
</div>

<div id="outline-container-orgf23b787" class="outline-3">
<h3 id="orgf23b787"><span class="section-number-3">1.9</span> Exercício 4</h3>
<div class="outline-text-3" id="text-1-9">
<p>
Crie a página login.php que recebe o nome, o email e a senha de um usuário, verifique se são iguais à:
</p>

<pre class="example">
$_GET['email'] == 'fulano@aluno.ifsp.edu.br' &amp;&amp; $_GET['senha'] == '654321'
</pre>

<p>
Substitua <b>fulano</b> por seu primeiro nome e <b>654321</b> por outra combinação de senha.
</p>

<p>
Se o email e a senha digitados forem corretos, ajuste uma variável em $_SESSION atribuindo o valor do nome e exiba o nome do usuário em todas as páginas do exercício 2.
</p>

<pre class="example">
echo "Olá, {$_SESSION['nome']}!";
</pre>
</div>
</div>
</div>
</div>
<div id="postamble" class="status">
<p class="date">Created: 2019-09-10 ter 22:02</p>
<p class="validation"><a href="http://validator.w3.org/check?uri=referer">Validate</a></p>
</div>
</body>
</html>
