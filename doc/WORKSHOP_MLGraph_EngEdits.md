<table>
<thead>
<tr class="header">
<th><table>
<tbody>
<tr class="odd">
<td><p>Machine Learning Workshop with Oracle Graph</p>
<h1 id="section"></h1>
<h1 id="contents" class="TOC-Heading">Contents</h1>
<p><a href="#about-this-workshop">About This Workshop 3</a></p>
<p><a href="#workshop-prerequisites">Workshop prerequisites: 3</a></p>
<p><a href="#workshop-details">Workshop details: 3</a></p>
<p><a href="#scenario-explanation">Scenario Explanation 4</a></p>
<p><a href="#scenario-solution">Scenario Solution 4</a></p>
<p><a href="#workshop-journey-map">Workshop Journey Map 5</a></p>
<p><a href="#step-1-convert-relational-data-model-to-graph-data-model.">Step 1: Convert Relational Data Model to Graph Data Model. 6</a></p>
<p><a href="#step-2-use-apache-zeppelin-to-access-graph-data-model.">Step 2: Use Apache Zeppelin to access Graph Data Model. 12</a></p>
<p><a href="#step-3-use-pypgx-to-access-graph-data-model.">Step 3: Use PyPGX to access Graph Data Model. 15</a></p>
<p><a href="#step-4-use-algorithm-your-graph-data-model.">Step 4: Use Algorithm your Graph Data Model. 19</a></p>
<p><a href="#step-5-use-open-source-vis.js-to-visualize-your-graph-data-model.">Step 5: Use Open Source Vis.JS to visualize your Graph Data Model. 22</a></p>
<p><a href="#step-6-use-graph-ui-to-visualize-your-graph-data-model.">Step 6: Use Graph UI to visualize your Graph Data Model. 25</a></p>
<p><a href="#conclusions">Conclusions 31</a></p>
<h1 id="section-1"></h1>
<h1 id="section-2"></h1>
<h1 id="section-3"></h1>
<h1 id="section-4"></h1>
<h1 id="section-5"></h1>
<p>Explore how to build a Bank Fraud Detection engine using Oracle Graph on a real-world dataset residing in Oracle Autonomous Database.</p>
<h1 id="about-this-workshop">About This Workshop</h1>
<p>This workshop walks you through the steps to build a Bank Fraud Detection engine using Oracle Graph on a real-world dataset residing in Oracle Autonomous Database. You will access to a bank dataset, use Graph Server, create a Property Graph data model, perform graph visualization and graph analysis.</p>
<h1 id="workshop-prerequisites">Workshop prerequisites:</h1>
<ul>
<li><blockquote>
<p>Familiarity with Database is desirable, but not required</p>
</blockquote></li>
<li><blockquote>
<p>Some understanding of cloud and database terms is helpful</p>
</blockquote></li>
<li><blockquote>
<p>Familiarity with Oracle Cloud Infrastructure (OCI) is helpful</p>
</blockquote></li>
<li><blockquote>
<p>Familiarity with Graph technologies is helpful</p>
</blockquote></li>
<li><blockquote>
<p>Internet connection to use a web browser.</p>
</blockquote></li>
</ul>
<h1 id="workshop-details">Workshop details:</h1>
<p>Together with Oracle experts you will be able to learn and experience the advantages of Oracle's converged database for transactional uses with advanced graph analytics, which will help you innovate, improving the management, efficiency and performance of your data models.<br />
<br />
In this workshop, we will teach you to develop graph analytics (Property Graph) and you will learn about the tools to transform a relational model into a graph. You will explore the use of the PGQL query language, the included advanced analytics algorithms, and the GraphViz visualization tool.We will also teach you to connect opensource graph tool like Vis.js or D3.js to our property graph data model.</p>
<h1 id="section-6"></h1>
<h1 id="scenario-explanation">Scenario Explanation</h1>
<p>While no fraud prevention measures can ever be perfect, significant opportunity for improvement lies in looking beyond the individual data points, to the connections that link them. Oftentimes these connections go unnoticed until it is too late— something that is unfortunate, as these connections oftentimes hold the best clues.</p>
<p>While the exact details behind each first-party fraud collusion vary from operation to operation, the pattern below illustrates how fraud rings commonly operate:</p>
<ul>
<li><p>A group of two or more people organize into a fraud ring</p></li>
<li><p>The ring shares a subset of legitimate contact information, for example phone numbers and addresses, combining them to create a number of synthetic identities</p></li>
<li><p>Ring members open accounts using these synthetic identities</p></li>
<li><p>New accounts are added to the original ones: unsecured credit lines, credit cards, overdraft protection, personal loans, etc.</p></li>
<li><p>The accounts are used as normally, with regular purchases and timely payments</p></li>
<li><p>Banks increase the revolving credit lines over time, due to the observed responsible credit behavior</p></li>
<li><p>One day the ring “busts out”, coordinating their activity, maxing out all of their credit lines, and disappearing</p></li>
<li><p>Sometimes fraudsters will go a step further and bring all of their balances to zero using fake checks immediately before the prior step, doubling the damage</p></li>
<li><p>Collections processes ensue, but agents are never able to reach the fraudster</p></li>
<li><p>The uncollectible debt is written off</p></li>
</ul>
<h1 id="scenario-solution">Scenario Solution</h1>
<p>Oracle Graph databases offer new methods of uncovering fraud rings and other sophisticated scams with a high-level of accuracy, and are capable of stopping advanced fraud scenarios in real-time.</p>
<p>We will use the Oracle Graph Database solution in order to resolve this problem.</p>
<p>Augmenting one’s existing fraud detection infrastructure to support ring detection can be done by running appropriate entity link analysis queries using a graph database, and running checks during key stages in the customer &amp; account lifecycle, such as:</p>
<ul>
<li><p>At the time the account is created</p></li>
<li><p>During an investigation</p></li>
<li><p>As soon as a credit balance threshold is hit</p></li>
<li><p>When a check is bounced</p></li>
</ul>
<p>Real-time graph traversals tied to the right kinds of events can help banks identify probable fraud rings: during or even before the Bust-Out occurs.</p>
<h1 id="workshop-journey-map">Workshop Journey Map</h1>
<p>To demonstrate the Oracle Graph functionalities, the workshop has been divided in different steps.</p>
<p>The documentation for this workshop has been published in the next github account:</p>
<p><a href="https://github.com/operard/mlgraph">https://github.com/operard/mlgraph</a></p>
<p>You can find the Documentation of Oracle Graph in the next URL:</p>
<p><a href="https://docs.oracle.com/cd/E56133_01/latest/prog-guides/index.html">https://docs.oracle.com/cd/E56133_01/latest/prog-guides/index.html</a></p>
<p>The documentation for PGQL (Property Graph Query Language) is available in the next URLs:</p>
<p><a href="https://pgql-lang.org/">https://pgql-lang.org/</a></p>
<p><a href="https://github.com/oracle/pgql-lang">https://github.com/oracle/pgql-lang</a></p>
<p>Each developer will use an account to access to the Oracle Graph Lab:</p>
<p>User: <strong>workshopxxx</strong> (xxx between 001 to 100)</p>
<p>Pwd: <strong>welcome1</strong></p>
<p>The url to access to the Oracle Graph Lab is:</p>
<p><a href="https://bdabastion.sceceps.com/wsxxx/">https://bdabastion.sceceps.com/wsxxx/</a></p>
<p>The password to access to the Lab environment is: “<strong>welcome1</strong>”</p>
<h2 id="step-1-convert-relational-data-model-to-graph-data-model.">Step 1: Convert Relational Data Model to Graph Data Model.</h2>
<p>The bank stores the Customers data in a relational Data Model. The Banking or financial Data model stores the next information:</p>
<ul>
<li><p>Customers</p></li>
<li><p>Accounts</p></li>
<li><p>Credit Cards</p></li>
<li><p>Unsecured Loans</p></li>
</ul>
<p>The relational 3FN data model below represents how the data actually looks to the oracle database:</p>
<p>CREATE PROPERTY GRAPH bank</p>
<p>VERTEX TABLES (</p>
<p>ACCOUNTS KEY(UNIQUEID) PROPERTIES ALL COLUMNS,</p>
<p>CUSTOMERS as CUST KEY(UNIQUEID) PROPERTIES (FIRSTNAME,LASTNAME),</p>
<p>ADDRESS KEY(STREET,CITY,STATE,ZIPCODE) PROPERTIES (STREET,CITY,STATE,ZIPCODE),</p>
<p>PHONENUMBERS KEY(PHONENUMBER) PROPERTIES (PHONENUMBER),</p>
<p>SSN KEY(SSN) PROPERTIES ALL COLUMNS,</p>
<p>CREDITCARDS KEY(UNIQUEID) PROPERTIES ALL COLUMNS,</p>
<p>UNSECUREDLOANS KEY(UNIQUEID) PROPERTIES ALL COLUMNS</p>
<p>)</p>
<p>EDGE TABLES (</p>
<p>ACCOUNTS SOURCE KEY(UNIQUEID) REFERENCES CUST DESTINATION KEY(UNIQUEID) REFERENCES ACCOUNTS LABEL HAS_BANKACCOUNT,</p>
<p>CUST_ADDRESS SOURCE KEY(UNIQUEID) REFERENCES CUST DESTINATION KEY(STREET,CITY,STATE,ZIPCODE) REFERENCES ADDRESS LABEL HAS_ADDRESS,</p>
<p>CUST_PHONENUMBERS SOURCE KEY(UNIQUEID) REFERENCES CUST DESTINATION KEY(PHONENUMBER) REFERENCES PHONENUMBERS</p>
<p>LABEL HAS_PHONENUMBER,</p>
<p>CUST_SSN SOURCE KEY(UNIQUEID) REFERENCES CUST DESTINATION KEY(SSN) REFERENCES SSN</p>
<p>LABEL HAS_SSN,</p>
<p>CREDITCARDS SOURCE KEY(UNIQUEID) REFERENCES CUST DESTINATION KEY(UNIQUEID) REFERENCES CREDITCARDS</p>
<p>LABEL HAS_CREDITCARDS,</p>
<p>UNSECUREDLOANS SOURCE KEY(UNIQUEID) REFERENCES CUST DESTINATION KEY(UNIQUEID) REFERENCES UNSECUREDLOANS</p>
<p>LABEL HAS_UNSECUREDLOANS</p>
<p>);</p>
<p>In order to create the Graph Data Model (Property Graph Data Model), we will use the <strong>SQLCL</strong> Tool of Oracle Database.</p>
<p>To execute this tool, we will open the Shell Terminal from jupyter tool:</p>
<p><img src="media/image4.png" style="width:6.76806in;height:1.86736in" /></p>
<p>And Jupyter opens the next terminal:</p>
<p>Now, we can execute the next command:</p>
<p>/opt/sqlcl/bin/sql workshop<strong>xxx</strong>/welcome1@orclpdb</p>
<p>Check tables in your schema:</p>
<p>select table_name from user_tables;</p>
<p>Now, we will activate the PGQL language inside the SQL:</p>
<p>pgql auto on</p>
<p>Create the property graph schema from Relational Data Model:</p>
<p>CREATE PROPERTY GRAPH bank  VERTEX TABLES (    ACCOUNTS KEY(UNIQUEID) PROPERTIES ALL COLUMNS,    CUSTOMERS as CUST KEY(UNIQUEID) PROPERTIES (FIRSTNAME,LASTNAME),    ADDRESS KEY(STREET,CITY,STATE,ZIPCODE) PROPERTIES (STREET,CITY,STATE,ZIPCODE),    PHONENUMBERS KEY(PHONENUMBER) PROPERTIES (PHONENUMBER),    SSN KEY(SSN) PROPERTIES ALL COLUMNS,    CREDITCARDS KEY(UNIQUEID) PROPERTIES ALL COLUMNS,    UNSECUREDLOANS KEY(UNIQUEID) PROPERTIES ALL COLUMNS  )  EDGE TABLES (   ACCOUNTS     SOURCE KEY(UNIQUEID) REFERENCES CUST     DESTINATION KEY(UNIQUEID) REFERENCES ACCOUNTS     LABEL HAS_BANKACCOUNT,   CUST_ADDRESS    SOURCE KEY(UNIQUEID) REFERENCES CUST     DESTINATION KEY(STREET,CITY,STATE,ZIPCODE) REFERENCES ADDRESS     LABEL HAS_ADDRESS,   CUST_PHONENUMBERS    SOURCE KEY(UNIQUEID) REFERENCES CUST     DESTINATION KEY(PHONENUMBER) REFERENCES PHONENUMBERS     LABEL HAS_PHONENUMBER,   CUST_SSN    SOURCE KEY(UNIQUEID) REFERENCES CUST     DESTINATION KEY(SSN) REFERENCES SSN     LABEL HAS_SSN,   CREDITCARDS    SOURCE KEY(UNIQUEID) REFERENCES CUST     DESTINATION KEY(UNIQUEID) REFERENCES CREDITCARDS     LABEL HAS_CREDITCARDS,   UNSECUREDLOANS    SOURCE KEY(UNIQUEID) REFERENCES CUST     DESTINATION KEY(UNIQUEID) REFERENCES UNSECUREDLOANS     LABEL HAS_UNSECUREDLOANS  );</p>
<p>Now you can go out PGQL in order to check the Property Graph Data Model:</p>
<p>pgql auto off</p>
<p>Check tables in your schema:</p>
<p>select table_name from user_tables;</p>
<p>You can see that the “bank” property graph Data Model has created new tables in your database Schema:</p>
<ul>
<li><p>BANKGE$</p></li>
<li><p>BANKGT$</p></li>
<li><p>BANKIT$</p></li>
<li><p>BANKSS$</p></li>
<li><p>BANKVD$</p></li>
<li><p>BANKVT$</p></li>
</ul>
<p>Now, we will activate the PGQL language inside the SQL in order to delete the Graph Data Model created “BANK”:</p>
<p>pgql auto on</p>
<p>You can delete the Graph Data Model using the next commands (change the XXX by your workshop user ID):</p>
<p>/opt/sqlcl/bin/sql workshopXXX/welcome1@orclpdb</p>
<p>PGQL AUTO ON</p>
<p>DROP PROPERTY GRAPH BANK;</p>
<p>PGQL AUTO OFF</p>
<p>EXIT;</p>
<p>You can create your property graph Data Model „BANK“ using the next command line:</p>
<p>/opt/sqlcl/bin/sql workshopXXX/welcome1@orclpdb @pgbank_create.sql</p>
<h2 id="step-2-use-apache-zeppelin-to-access-graph-data-model.">Step 2: Use Apache Zeppelin to access Graph Data Model.</h2>
<p>Apache Zeppelin is an open source framework to develop notebooks using different programming languages using different interpreters available in the next URL:</p>
<p><a href="http://zeppelin.apache.org/">http://zeppelin.apache.org/</a></p>
<p>All users “workshopXXX” have been distributed in different Labs:</p>
<table>
<thead>
<tr class="header">
<th><strong>Users</strong></th>
<th><strong>Zeppelin URL</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Workshop001 to workshop020</td>
<td>https://bdabastion.sceceps.com/zp1<strong>/</strong></td>
</tr>
<tr class="even">
<td>Workshop021 to workshop040</td>
<td>https://bdabastion.sceceps.com/zp2<strong>/</strong></td>
</tr>
<tr class="odd">
<td>Workshop041 to workshop060</td>
<td>https://bdabastion.sceceps.com/zp3<strong>/</strong></td>
</tr>
<tr class="even">
<td>Workshop061 to workshop080</td>
<td>https://bdabastion.sceceps.com/zp4<strong>/</strong></td>
</tr>
<tr class="odd">
<td>Workshop081 to workshop100</td>
<td>https://bdabastion.sceceps.com/zp5<strong>/</strong></td>
</tr>
</tbody>
</table>
<p>Using the url for your workshop user, you should access to the next Apache Zeppelin page:</p>
<p><img src="media/image9.png" style="width:6.76806in;height:1.96806in" /></p>
<p>Click on “login” button and Use your user “workshopXXX”.</p>
<p><img src="media/image10.png" style="width:3.42715in;height:1.73432in" /></p>
<p>Select the notebook “<strong>Bank Ring Analysis</strong>” in the Folder for your user “workshopXXX”.</p>
<p><img src="media/image11.png" style="width:6.76806in;height:4.41389in" /></p>
<p>Execute each paragraph in this notebook “Step By Step” until the paragraph “First step, look for account sharing contact details: phone number, SSN or address,”.</p>
<p>You can see how you can program in Groovy language or Java Language. The interpreter used by PGX (Property graph Engine) from Oracle Graph is a Groovy/Java interpreter.</p>
<p>To load the graph in Memory from the Graph Data Model, you could use the next code:</p>
<p>%pgx</p>
<p>import oracle.pgx.common.types.*</p>
<p>builder.setUsername(user);</p>
<p>builder.setPassword(pass);</p>
<p>// Read the Graph Name created previously</p>
<p>builder.setName("bank");</p>
<p>builder.addVertexProperty("FIRSTNAME", PropertyType.STRING);</p>
<p>builder.addVertexProperty("LASTNAME", PropertyType.STRING);</p>
<p>builder.addVertexProperty("UNIQUEID", PropertyType.STRING);</p>
<p>builder.addVertexProperty("SSN", PropertyType.STRING);</p>
<p>builder.addVertexProperty("PHONENUMBER", PropertyType.STRING);</p>
<p>builder.addVertexProperty("BALANCE", PropertyType.DOUBLE);</p>
<p>builder.addVertexProperty("APR", PropertyType.DOUBLE);</p>
<p>builder.addVertexProperty("LOANAMOUNT", PropertyType.DOUBLE);</p>
<p>builder.addVertexProperty("STREET", PropertyType.STRING);</p>
<p>builder.addVertexProperty("STATE", PropertyType.STRING);</p>
<p>builder.addVertexProperty("ZIPCODE", PropertyType.STRING);</p>
<p>builder.addVertexProperty("CITY", PropertyType.STRING);</p>
<p>builder.addVertexProperty("ACCOUNTNUMBER", PropertyType.STRING);</p>
<p>builder.addVertexProperty("LIMIT", PropertyType.DOUBLE);</p>
<p>builder.addVertexProperty("SECURITYCODE", PropertyType.STRING);</p>
<p>builder.addVertexProperty("EXPIRATIONDATE", PropertyType.TIMESTAMP);</p>
<p>builder.setLoadVertexLabels(true);</p>
<p>builder.setLoadEdgeLabel(true);</p>
<p>builder.setKeystoreAlias("alias");</p>
<p>The name “<strong>bank</strong>” used in this code paragraph is depending on your Graph Data Model, you have created in the Step1.</p>
<h2 id="step-3-use-pypgx-to-access-graph-data-model.">Step 3: Use PyPGX to access Graph Data Model.</h2>
<p>All users “workshopXXX” have been distributed in different Labs:</p>
<table>
<thead>
<tr class="header">
<th><strong>Users</strong></th>
<th><strong>Jupyter URL</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Workshop001 to workshop020</td>
<td>https://bdabastion.sceceps.com/wsXXX</td>
</tr>
<tr class="even">
<td>Workshop021 to workshop040</td>
<td>https://bdabastion.sceceps.com/wsXXX</td>
</tr>
<tr class="odd">
<td>Workshop041 to workshop060</td>
<td>https://bdabastion.sceceps.com/wsXXX</td>
</tr>
<tr class="even">
<td>Workshop061 to workshop080</td>
<td>https://bdabastion.sceceps.com/wsXXX</td>
</tr>
<tr class="odd">
<td>Workshop081 to workshop100</td>
<td>https://bdabastion.sceceps.com/wsXXX</td>
</tr>
</tbody>
</table>
<p>You can find the documentation of PyPGX in the next URL:</p>
<p><a href="https://docs.oracle.com/cd/E56133_01/latest/pythondocs/index.html">https://docs.oracle.com/cd/E56133_01/latest/pythondocs/index.html</a></p>
<p>With your workshop user, let’s connect to <a href="https://bdabastion.sceceps.com/wsXXX">https://bdabastion.sceceps.com/wsXXX</a>.</p>
<p><img src="media/image12.png" style="width:6.76806in;height:2.71042in" /></p>
<p>To check how you can access to the Graph Data Model, select the notebook “PGX.analysis.bank.ipynb”.</p>
<p><img src="media/image13.png" style="width:6.76806in;height:3.47986in" /></p>
<p>Execute all the different paragraphs of this notebook “step by step”.</p>
<p>To load the graph from Oracle Database, we have created a metadata definition “bank.json” where you can choose the vertex and edges you want to load in Memory:</p>
<p>{</p>
<p>"db_engine": "RDBMS",</p>
<p>"vertex_id_type": "long",</p>
<p>"error_handling": {},</p>
<p>"name": "bank",</p>
<p>"vertex_props": [</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "FIRSTNAME",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "LASTNAME",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "UNIQUEID",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "SSN",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "PHONENUMBER",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "BALANCE",</p>
<p>"type": "double"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "APR",</p>
<p>"type": "double"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "LOANAMOUNT",</p>
<p>"type": "double"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "STREET",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "STATE",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "ZIPCODE",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "CITY",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "ACCOUNTNUMBER",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "LIMIT",</p>
<p>"type": "double"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "SECURITYCODE",</p>
<p>"type": "string"</p>
<p>},</p>
<p>{</p>
<p>"dimension": 0,</p>
<p>"name": "EXPIRATIONDATE",</p>
<p>"type": "timestamp"</p>
<p>}</p>
<p>],</p>
<p>"loading": {</p>
<p>"load_vertex_labels": true,</p>
<p>"load_edge_label": true</p>
<p>},</p>
<p>"edge_props": [],</p>
<p>"attributes": {},</p>
<p>"format": "pg"</p>
<p>}</p>
<p><img src="media/image14.png" style="width:6.76806in;height:1.43333in" /></p>
<p>Now you can compare with the loading mechanism in Apache Zeppelin notebook:</p>
<p>%pgx</p>
<p>import oracle.pgx.common.types.*</p>
<p>builder.setUsername(user);</p>
<p>builder.setPassword(pass);</p>
<p>// Read the Graph Name created previously</p>
<p>builder.setName("bank");</p>
<p>builder.addVertexProperty("FIRSTNAME", PropertyType.STRING);</p>
<p>builder.addVertexProperty("LASTNAME", PropertyType.STRING);</p>
<p>builder.addVertexProperty("UNIQUEID", PropertyType.STRING);</p>
<p>builder.addVertexProperty("SSN", PropertyType.STRING);</p>
<p>builder.addVertexProperty("PHONENUMBER", PropertyType.STRING);</p>
<p>builder.addVertexProperty("BALANCE", PropertyType.DOUBLE);</p>
<p>builder.addVertexProperty("APR", PropertyType.DOUBLE);</p>
<p>…etc….</p>
<h2 id="step-4-use-algorithm-your-graph-data-model.">Step 4: Use Algorithm your Graph Data Model.</h2>
<p>You can check that this Dataset has been prepared to generate some rings in the data:</p>
<p><img src="media/image15.png" style="width:6.6676in;height:3.75052in" /></p>
<p>It is not a clean dataset and now the objective is to use the PGQL query language in order to detect the different rings in the data.</p>
<p>You can analyze the Entities Links between the different Vertex:</p>
<p><img src="media/image16.png" style="width:6.76806in;height:2.70625in" /></p>
<p>You can check the Financial Risk for possible Fraud Ring (PyPGX).</p>
<p><img src="media/image17.png" style="width:6.76806in;height:2.63125in" /></p>
<p>You can compare with Apache Zeppelin Notebook execution using the Groovy language:</p>
<p><img src="media/image18.png" style="width:6.76806in;height:2.16389in" /></p>
<p><img src="media/image19.png" style="width:6.76806in;height:2.70556in" /></p>
<h2 id="step-5-use-open-source-vis.js-to-visualize-your-graph-data-model.">Step 5: Use Open Source Vis.JS to visualize your Graph Data Model.</h2>
<p>Connect to Jupyter Notebook using your workshop user (change the XXX by your userid 001 to 100):</p>
<p><a href="https://bdabastion.sceceps.com/wsXXX">https://bdabastion.sceceps.com/wsXXX</a></p>
<p><img src="media/image12.png" style="width:6.76806in;height:2.71042in" /></p>
<p>Execute the notebook “<strong>PGX.visjs.Bank.ipynb</strong>”.</p>
<p>In this notebook, we are using the Python Library “pyvis” where the open source JavaScript Library Vis.JS has been embedded.</p>
<p><a href="https://visjs.org/">https://visjs.org/</a></p>
<p>In this open source library, a widget “Network” has been implemented in order to represent a graph in JavaScript component.</p>
<p><a href="https://visjs.github.io/vis-network/docs/network/">https://visjs.github.io/vis-network/docs/network/</a></p>
<p>Execute Queries in order to create Nodes List and Edges List for Vis.JS:</p>
<p><img src="media/image20.png" style="width:6.76806in;height:3.33819in" /></p>
<p>Using Network:</p>
<p><img src="media/image21.png" style="width:6.76806in;height:3.04236in" /></p>
<p>Using NetworkX:</p>
<p><img src="media/image22.png" style="width:6.76806in;height:3.29861in" /></p>
<p><img src="media/image23.png" style="width:6.01052in;height:5.63486in" /></p>
<h2 id="step-6-use-graph-ui-to-visualize-your-graph-data-model.">Step 6: Use Graph UI to visualize your Graph Data Model.</h2>
<p>Oracle Graph includes an UI Visualizer for PGX using JavaScript libraries.</p>
<p>You can access to this tool using the next URL:</p>
<p><a href="https://bdabastion.sceceps.com/ui">https://bdabastion.sceceps.com/ui</a></p>
<p>Use the next generic information to login to the tool “PGX Visualizer”:</p>
<p>User: bankuser</p>
<p>Pwd: welcome1</p>
<p><img src="media/image24.png" style="width:3.42498in;height:6.19835in" /></p>
<p>Select the “global_bank” Graph Name in the combobox.</p>
<p>Copy the next query to select all relationships (edges):</p>
<p>SELECT e</p>
<p>FROM MATCH ()-[e]-&gt;()</p>
<p>LIMIT 100</p>
<p>In order to draw a visualization, you can limit the number of results.</p>
<p>Execute the next button “Run Query”:</p>
<p><img src="media/image25.png" style="width:6.76806in;height:1.18542in" /></p>
<p>The PGX Visualizer using a Javascript library draws the Vertex and Edges list in the UI:</p>
<p><img src="media/image26.png" style="width:6.76806in;height:3.94792in" /></p>
<p>By default, the PGX Visualizer generate a visualization for Vertex and Edges and you can customize the visualization using the toolbar button on the right side.</p>
<p>You can download the next JSON Configuration file from github repository “<a href="https://github.com/operard/mlgraph/blob/main/graphviz/bank_settings_20210315.json">https://github.com/operard/mlgraph/blob/main/graphviz/bank_settings_20210315.json</a>”</p>
<p>{"version":6,"theme":"light","height":300,"similarEdges":"keep","edgeMarker":"arrow","vertexGeometry":"sphere","antiAlias":true,"floorGrid":true,"edgesGeometry":true,"enable3DLayout":false,"selectedPropZ":"","valueRangePropZ":0.5,"sortPropZ":"descending","filters":[{"_id":1615824847813,"type":"styling","enabled":true,"conditions":{"operator":"and","conditions":[{"property":"label","operator":"=","value":"CUST"}]},"component":"vertex","target":"vertex","properties":{"icons":["fa-user"],"iconColors":["white"],"label":["FIRSTNAME"]}},{"_id":1615824870065,"type":"styling","enabled":true,"conditions":{"operator":"and","conditions":[]},"component":"edge","target":"edge","properties":{"label":["label"]}},{"_id":1615824919274,"type":"styling","enabled":true,"conditions":{"operator":"and","conditions":[{"property":"label","operator":"=","value":"PHONENUMBERS"}]},"component":"vertex","target":"vertex","properties":{"colors":["black"],"icons":["fa-phone"],"iconColors":["white"],"label":["PHONENUMBER"]}},{"_id":1615828536887,"type":"styling","enabled":true,"conditions":{"operator":"and","conditions":[{"property":"label","operator":"=","value":"ACCOUNTS"}]},"component":"vertex","target":"vertex","properties":{"colors":["red"],"icons":["fa-building"],"iconColors":["white"],"label":["ACCOUNTNUMBER"]}},{"_id":1615828630015,"type":"styling","enabled":true,"conditions":{"operator":"and","conditions":[{"property":"label","operator":"=","value":"SSN"}]},"component":"vertex","target":"vertex","properties":{"colors":["rgb(163, 163, 57)"],"icons":["fa-hospital-o"],"iconColors":["white"],"label":["SSN"]}},{"_id":1615828721839,"type":"styling","enabled":true,"conditions":{"operator":"and","conditions":[{"property":"label","operator":"=","value":"CREDITCARDS"}]},"component":"vertex","target":"vertex","properties":{"colors":["rgb(134, 56, 236)"],"icons":["fa-id-card"],"iconColors":["white"],"label":["ACCOUNTNUMBER"]}}],"smartExpands":[],"smartGroups":[],"vertexLabelProperty":null,"edgeLabelProperty":null,"vertexLabelOrientation":"bottom","vertexPositions":[{"id":"6915093083595417275","x":0.39905679562582147,"y":0.418391158327987},{"id":"565234722105082376","x":0.3067477945341144,"y":0.5443462008779054},{"id":"3824048412016813344","x":0.4270791709572325,"y":0.5573121611403969},{"id":"6696452419939143867","x":0.7238514251596001,"y":0.3256123683876622},{"id":"524214483973154798","x":0.3601054994781409,"y":0.5830259232993977},{"id":"3265555656079332997","x":0.4066149976091672,"y":0.2959708075190381},{"id":"7012961393350504935","x":0.5648861255774357,"y":0.7062724132268348},{"id":"4090088222170435427","x":0.43924106346227515,"y":0.5299831301660705},{"id":"879672803699099970","x":0.21502363217389478,"y":0.4129769688425543},{"id":"2074598160484072345","x":0.26778067482998424,"y":0.614227566319002},{"id":"6669874926900192849","x":0.5662744688052275,"y":0.38801565442687086},{"id":"7396233240736154172","x":0.32262023232776155,"y":0.7858366029268257},{"id":"8564415915979133027","x":0.19419848375701743,"y":0.22732719287590866},{"id":"516309596472504986","x":0.5586385810523725,"y":0.15400333177983858},{"id":"6180573890730454984","x":0.839778084680218,"y":0.19612554985630437},{"id":"6840400127837741695","x":0.8619915763248872,"y":0.4582193512209805},{"id":"3483432232742040934","x":0.7849385271824407,"y":0.6953518381699731},{"id":"6281001637277489523","x":0.6655410095923434,"y":0.7624353706621224}],"pageSize":100,"selectedPage":0,"charLimit":10,"truncateLabel":false,"showTitle":true,"dimension":"2d","layout":"force","layoutProperties":{"circle":{"avoidOverlap":true,"radius":40},"grid":{"avoidOverlap":true,"rows":5,"columns":5},"concentric":{"avoidOverlap":true,"minimumVertexSpacing":10},"force":{"edgeDistance":120,"forceStrength":-30,"vertexPadding":40,"velocityDecay":0.3},"force3D":{"attractionMultiplier":20,"repulsionMultiplier":0.2},"geographical":{"latitude":"latitude","longitude":"longitude"},"hierarchical":{"rankDirection":"TB","ranker":"network-simplex","align":"","vertexSeparation":{"value":0,"enabled":false},"edgeSeparation":{"value":0,"enabled":false},"rankSeparation":{"value":0,"enabled":false}},"radial":{"arcDegree":360,"startingPoint":"left","packing":1,"intelligentSeparation":true}},"animateChanges":true,"liveSearch":{"enabled":false,"enabledTypes":[],"selectedColumns":[],"value":"","location":0,"distance":100,"maxPatternLength":32,"minMatchCharLength":1,"advancedSettingsToggle":false,"disabledSelectedColumns":[]},"graphAction":{"enabled":true,"graphName":"bank_21","lastRun":0,"metadata":{"vertexProperties":[],"edgeProperties":[]},"stack":[],"index":0,"numberOfHops":1,"smartExpand":0,"smartGroup":0},"interactionMode":"zoom","networkEvolution":{"enabled":false,"vertexProperty":"id","vertexEndProperty":"","dataType":"int","axis":"vertices","overview":"on","height":100,"overviewChartType":"bar","valuesToExclude":[],"valuesToExcludeType":"hideBoth","stepSize":0,"edgeProperty":"id","edgeEndProperty":"","playTimeout":1000,"playStep":1,"advancedSettingsToggle":false},"stickyVertices":true,"annotationMode":false,"fitToScreen":false,"viewTransform":[[-220.75572591785055,-71.71488606101718,1.33262346325533,1081]],"showLegend":true,"visibleGraphMode":{"enabled":false,"name":""},"width":100}</p>
<p>You can upload this JSON configuration file “bank_settings_20210315.json” using the “Load Settings” button.</p>
<p><img src="media/image28.png" style="width:6.76806in;height:3.71111in" /></p>
<p><img src="media/image29.png" style="width:6.76806in;height:3.30139in" /></p></td>
</tr>
</tbody>
</table></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td></td>
</tr>
<tr class="even">
<td><h1 id="conclusions">Conclusions</h1>
<p>In this workshop, we have seen how you can reuse and convert a 3FN relational data model in order to apply Queries and Machine Learning algorithms using the same Oracle Database.</p>
<p>This functionality is available in order to apply fast use cases on the relationships between entities.</p>
<p>You can continue to implement Oracle Graph use cases using the free labs available in the next URLs:</p>
<ul>
<li><p>Oracle Property Graph for Real-Time Recommendations Workshop</p></li>
</ul>
<p><a href="https://apexapps.oracle.com/pls/apex/dbpm/r/livelabs/view-workshop?wid=754">https://apexapps.oracle.com/pls/apex/dbpm/r/livelabs/view-workshop?wid=754</a></p>
<ul>
<li><p>Analyze and Visualize Property Graphs with Oracle Database Workshop</p></li>
</ul>
<p><a href="https://apexapps.oracle.com/pls/apex/dbpm/r/livelabs/view-workshop?wid=687">https://apexapps.oracle.com/pls/apex/dbpm/r/livelabs/view-workshop?wid=687</a></p>
<ul>
<li><p>Getting started with Oracle Property Graph on Docker Workshop</p></li>
</ul>
<p><a href="https://apexapps.oracle.com/pls/apex/dbpm/r/livelabs/view-workshop?wid=712">https://apexapps.oracle.com/pls/apex/dbpm/r/livelabs/view-workshop?wid=712</a></p>
<p>Other Labs in Machine Learning, AI, Data Management, …etc… are available in the next URL:</p></td>
</tr>
<tr class="odd">
<td><a href="https://apexapps.oracle.com/pls/apex/dbpm/r/livelabs/livelabs-workshop-cards?clear=100&amp;session=101956397438991">https://apexapps.oracle.com/pls/apex/dbpm/r/livelabs/livelabs-workshop-cards?clear=100&amp;session=101956397438991</a></td>
</tr>
</tbody>
</table>
