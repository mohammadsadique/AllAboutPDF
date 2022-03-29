# AllAboutPDF


## Size of PDF page can modify using @page style CSS
    @page{
        size: 600pt 960pt;
    }


## Header-Footer Repeat in every pages of PDF
    <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta http-equiv="X-UA-Compatible" content="IE=edge">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Carrier Invite</title>
        </head>
        <style>
            header {
                position: fixed;
                top: -55px;
                left: 25px; 
                right: 0px;
                height: 50px;

                /** Extra personal styles **/
                line-height: 35px;
            }
            footer {
                position: fixed; 
                bottom: -60px; 
                left: 0px; 
                right: 0px;
                height: 50px; 
                font-size: 20px !important;

                /** Extra personal styles **/
                text-align: center;
                line-height: 35px;
            }
            @page {
                margin: 100px 25px;
            }
            body{
                margin: 80px 30px 0px 30px;
            }
        </style>
        <body>
            <header>
                <img src="http://localhost:4200/assets/images/logo.png" alt="logo">
            </header>
            <footer>
                <span class="pagenum"></span>
            </footer>
            <main>
                Your content here...
            </main>
        </body>
    </html>
