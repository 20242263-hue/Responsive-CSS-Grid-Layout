
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Responsive Grid Page</title>

<style>

.container {
    width: 100%;
    margin: auto;
}

.row {
    display: flex;
    flex-wrap: wrap;
}

[class*="col-"] {
    padding: 10px;
}


.col-12 { width: 100%; }
.col-6 { width: 50%; }
.col-4 { width: 33.33%; }
.col-3 { width: 25%; }


@media (max-width: 768px) {
    .col-6, .col-4, .col-3 {
        width: 100%;
    }
}


.box {
    background: #e3e3e3;
    padding: 20px;
    border: 1px solid #ccc;
    font-size: 18px;
    border-radius: 5px;
}
</style>

</head>
<body>

<div class="container">

    
    <div class="row">
        <div class="col-12">
            <div class="box">Header</div>
        </div>
    </div>

    
    <div class="row">

        <div class="col-3">
            <div class="box">Sidebar</div>
        </div>

        <div class="col-9">
            <div class="box">
                <h3>Main Content</h3>

                <div class="row">
                    <div class="col-6">
                        <div class="box">Sub Content 1</div>
                    </div>

                    <div class="col-6">
                        <div class="box">Sub Content 2</div>
                    </div>
                </div>

            </div>
        </div>

    </div>

    
    <div class="row">
        <div class="col-12">
            <div class="box">Footer</div>
        </div>
    </div>

</div>

</body>
</html>
