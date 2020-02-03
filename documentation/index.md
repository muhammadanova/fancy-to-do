<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
  <meta name="description" content="">
  <meta name="author" content="">
  <meta name="keywords" content="">
  <title>Documentation Todo List</title>
  <link rel="shortcut icon" href="images/favicon.ico" type="image/x-icon">
  <link rel="stylesheet" type="text/css" href="fonts/font-awesome-4.3.0/css/font-awesome.min.css">
  <link rel="stylesheet" type="text/css" href="css/stroke.css">
  <link rel="stylesheet" type="text/css" href="css/bootstrap.css">
  <link rel="stylesheet" type="text/css" href="css/animate.css">
  <link rel="stylesheet" type="text/css" href="css/prettyPhoto.css">
  <link rel="stylesheet" type="text/css" href="css/style.css">
  <link rel="stylesheet" type="text/css" href="js/syntax-highlighter/styles/shCore.css" media="all">
  <link rel="stylesheet" type="text/css" href="js/syntax-highlighter/styles/shThemeRDark.css" media="all">
  <!-- CUSTOM -->
  <link rel="stylesheet" type="text/css" href="css/custom.css">
</head>
<body>
  <div id="wrapper">
    <div class="container">
      <section id="top" class="section docs-heading">
        <div class="row">
          <div class="col-md-12">
            <div class="big-title text-center">
              <h1>Todolist Documentation</h1>
              <p class="lead">Enjoyed!</p>
            </div>
          </div>
        </div>
        <hr>
      </section>
      <div class="row">
        <div class="col-md-3">
          <nav class="docs-sidebar" data-spy="affix" data-offset-top="300" data-offset-bottom="200" role="navigation">
            <ul class="nav">
              <li><a href="#top">Getting Started</a></li>
              <li><a href="#router">Router</a></li>
              <li><a href="#get-todos">GET Todos</a></li>
              <li><a href="#get-detail-todos">GET Detail Todos</a></li>
              <li><a href="#put-todos">PUT Todos</a></li>
              <li><a href="#post-todos">POST Todos</a></li>
              <li><a href="#delete-todos">DELETE Todos</a></li>
            </ul>
          </nav >
        </div>
        <div class="col-md-9">
          <section class="welcome">
            <div class="row">
              <div class="col-md-12 left-align">
                <h2 class="dark-text">Install</h2>
                <div class="row">
                  <div class="col-md-12 full">
                    <div class="terminal">
                      <ul>
                        <li>npm install express sequelize pg</li>
                      </ul>
                    </div>
                  </div>
                </div>
                <h2 class="dark-text">Running</h2>
                <div class="row">
                  <div class="col-md-12 full">
                    <div class="terminal">
                      <ul>
                        <li>npm run dev</li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </section>
          <section id="router" class="section">
            <div class="row">
              <div class="col-md-12 left-align">
                <h2 class="dark-text">Router <a href="#top">#back to top</a></h2>
              </div>
            </div>
            <div class="row">
              <div class="col-md-12">
                <h4>Router list</h4>
                <div class="intro1">
                  <ul>
                    <li>GET Todo List</li>
                    <li>GET Detail Todo List By ID</li>
                    <li>POST Todo List</li>
                    <li>PUT Todo List By ID</li>
                    <li>DELETE Todo List By ID</li>
                  </ul>
                </div>
              </div>
            </div>
          </section>
          <section id="get-todos" class="section">
            <div class="row">
              <div class="col-md-12 left-align">
                <h2 class="dark-text">GET TODOS<a href="#top">#back to top</a></h2>
              </div>
            </div>
            <div class="row">
              <div class="col-md-12">
                <h4>GET /todos Detail</h4>
                <p>Testing with Postman</p>
                <div class="intro1">
                  <ul>
                    <li>Method : GET</li>
                    <li>URL : http://localhost:3000/todos</li>
                  </ul>
                </div>
                <h6>Request Response : </h6>
                <pre class="brush: html; highlight: [2,4]">
                  [
                    {
                      "id": 1,
                      "title": "Install Express, Postgres, Sequelize",
                      "description": "Caranya dengan npm install express pg sequelize",
                      "status": 0,
                      "due_date": "2020-02-03T00:00:00.001Z",
                      "createdAt": "2020-02-03T11:29:33.093Z",
                      "updatedAt": "2020-02-03T11:29:33.093Z"
                    }
                  ]
                </pre>
              </div>
            </div>
          </section>
          <section id="get-detail-todos" class="section">
            <div class="row">
              <div class="col-md-12 left-align">
                <h2 class="dark-text">GET DETAIL TODOS<a href="#top">#back to top</a></h2>
              </div>
            </div>
            <div class="row">
              <div class="col-md-12">
                <h4>GET /todos/:id Detail</h4>
                <p>Testing with Postman</p>
                <div class="intro1">
                  <ul>
                    <li>Method : GET</li>
                    <li>URL : http://localhost:3000/todos/1</li>
                  </ul>
                </div>
                <h6>Request Response : </h6>
                <pre class="brush: html; highlight: [2,4]">
                  {
                    "id": 1,
                    "title": "Install Express, Postgres, Sequelize",
                    "description": "Caranya dengan npm install express pg sequelize",
                    "status": 0,
                    "due_date": "2020-02-03T00:00:00.001Z",
                    "createdAt": "2020-02-03T11:29:33.093Z",
                    "updatedAt": "2020-02-03T11:29:33.093Z"
                  }
                </pre>
              </div>
            </div>
          </section>
          <section id="put-todos" class="section">
            <div class="row">
              <div class="col-md-12 left-align">
                <h2 class="dark-text">PUT TODOS<a href="#top">#back to top</a></h2>
              </div>
            </div>
            <div class="row">
              <div class="col-md-12">
                <h4>PUT /todos Detail</h4>
                <p>Testing with Postman</p>
                <div class="intro1">
                  <ul>
                    <li>Method : PUT</li>
                    <li>URL : http://localhost:3000/todos/1</li>
                  </ul>
                </div>
                <h6>Request Header : </h6>
                <pre class="brush: html; highlight: [2,4]">
                  {
                    "Content-Type" : "application/json"
                  }
                </pre>
                <h6>Request Body : </h6>
                <pre class="brush: html; highlight: [2,4]">
                  {
                    "title": "Install EJS",
                    "description": "Caranya dengan npm install ejs",
                    "status": 0,
                    "due_date": "2020-02-03"
                  }
                </pre>
                <h6>Request Response : </h6>
                <pre class="brush: html; highlight: [2,4]">
                  {
                    "id": 1,
                    "title": "Install EJS",
                    "description": "Caranya dengan npm install ejs",
                    "status": 0,
                    "due_date": "2020-02-03T00:00:00.001Z",
                    "updatedAt": "2020-02-03T11:29:45.616Z",
                    "createdAt": "2020-02-03T11:29:45.616Z"
                  }
                </pre>
              </div>
            </div>
          </section>
          <section id="post-todos" class="section">
            <div class="row">
              <div class="col-md-12 left-align">
                <h2 class="dark-text">POST TODOS<a href="#top">#back to top</a></h2>
              </div>
            </div>
            <div class="row">
              <div class="col-md-12">
                <h4>POST /todos Detail</h4>
                <p>Testing with Postman</p>
                <div class="intro1">
                  <ul>
                    <li>Method : POST</li>
                    <li>URL : http://localhost:3000/todos</li>
                  </ul>
                </div>
                <h6>Request Header : </h6>
                <pre class="brush: html; highlight: [2,4]">
                  {
                    "Content-Type" : "application/json"
                  }
                </pre>
                <h6>Request Body : </h6>
                <pre class="brush: html; highlight: [2,4]">
                  {
                    "title": "Install Express JS, Postgres, Sequelize",
                    "description": "Caranya dengan npm install express postgres sequelize",
                    "status": 0,
                    "due_date": "2020-02-03"
                  }
                </pre>
                <h6>Request Response : </h6>
                <pre class="brush: html; highlight: [2,4]">
                  {
                    "id": 1,
                    "title": "Install Express JS, Postgres, Sequelize",
                    "description": "Caranya dengan npm install express postgres sequelize",
                    "status": 0,
                    "due_date": "2020-02-03T00:00:00.001Z",
                    "updatedAt": "2020-02-03T11:29:45.616Z",
                    "createdAt": "2020-02-03T11:29:45.616Z"
                  }
                </pre>
              </div>
            </div>
          </section>
          <section id="delete-todos" class="section">
            <div class="row">
              <div class="col-md-12 left-align">
                <h2 class="dark-text">DELETE TODOS<a href="#top">#back to top</a></h2>
              </div>
            </div>
            <div class="row">
              <div class="col-md-12">
                <h4>DELETE /todos</h4>
                <p>Testing with Postman</p>
                <div class="intro1">
                  <ul>
                    <li>Method : DELETE</li>
                    <li>URL : http://localhost:3000/todos/1</li>
                  </ul>
                </div>
                <h6>Request Response : </h6>
                <pre class="brush: html; highlight: [2,4]">
                  {
                    "id": 1,
                    "title": "Install EJS",
                    "description": "Caranya dengan npm install ejs",
                    "status": 0,
                    "due_date": "2020-02-03T00:00:00.001Z",
                    "createdAt": "2020-02-03T11:29:33.093Z",
                    "updatedAt": "2020-02-03T11:29:33.093Z"
                  }
                </pre>
              </div>
            </div>
          </section>
        </div>
      </div>
    </div>

    <script src="js/jquery.min.js"></script>
    <script src="js/bootstrap.min.js"></script>
    <script src="js/retina.js"></script>
    <script src="js/jquery.fitvids.js"></script>
    <script src="js/wow.js"></script>
    <script src="js/jquery.prettyPhoto.js"></script>

    <!-- CUSTOM PLUGINS -->
    <script src="js/custom.js"></script>
    <script src="js/main.js"></script>

    <script src="js/syntax-highlighter/scripts/shCore.js"></script>
    <script src="js/syntax-highlighter/scripts/shBrushXml.js"></script>
    <script src="js/syntax-highlighter/scripts/shBrushCss.js"></script>
    <script src="js/syntax-highlighter/scripts/shBrushJScript.js"></script>
</body>
</html>