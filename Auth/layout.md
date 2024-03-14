<div id="documentação">
    <div>
        <h1>AuthComponent</h1>
        <p>o componente <b>AuthComponent</b> utiliza do componente <b>LayoutAuthComponent</b> para renderizar o leu layout, mas <b>nada deve ser alterado dentro do LayoutAuthComponent</b>, tudo é setado dentro do póprio AuthComponent.</p>
    </div>
    <div>
        <h2>Layout</h2>
        <p>O componente <b>LayoutAuthComponent</b> por padrão tem um @input chamdo  <b>layout</b> que é uma string literal *"full"* ou um numero;</p>
        <table>
            <thead><tr><th>Full</th><th>Número</th><tr></thead>
            <tbody>
                <tr>
                    <td>
                        <p>O componente tocará as bordas do navegador.</p>
                        <pre><code>&lt;app-layout-auth [layout]="full"&gt;&lt;/app-layout-auth&gt;</code></pre>
                    </td>
                    <td>
                        <p>O componente tocará as bordas do navegador.</p>
                        <pre><code>&lt;app-layout-auth [layout]="20"&gt;&lt;/app-layout-auth&gt;</code></pre>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
    <div>
        <h2>Banner Lateral</h2>
        <p>componente <b>LayoutAuthComponent</b> pode renderizar com ou sem um banner lateral</p>
        <table>
            <thead><tr><th>SEM BANNER</th><th>COM BANNER</th><tr></thead>
            <tbody>
                <tr>
                    <td>
                        <p>apenas chamando o componente <b>LayoutAuthComponent<b></p>
                        <pre><code>&lt;app-layout-auth&gt;&lt;/app-layout-auth&gt;</code></pre>
                    </td>
                    <td>
                        <p>Adicine uma tag div com atributo banner</p>
                        <pre><code>&lt;app-layout-auth&gt
                            ;&lt;div banner&gt;&lt;/div&gt;
                        &lt;/app-layout-auth&gt;</code></pre>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
    <div>
        <h2>Banner Rotativo</h2>
        <p>O banner lateral tem a opção de ser rotativo com infinitos banners</p>
        <table>
            <thead><tr><th>BANNER ROTATICO</th><tr></thead>
            <tbody>
                <tr>
                    <td>
                        <p>O numero de divs com atributo banner virará automaticamente um banner rotativo</p>
                        <code>
                            &lt;app-layout-auth&gt;
                            <br/>&nbsp;&nbsp;&nbsp;&lt;div banner&gt;&lt;/div&gt;
                            <br/>&nbsp;&nbsp;&nbsp;&lt;div banner&gt;&lt;/div&gt;
                            <br/>&nbsp;&nbsp;&nbsp;&lt;div banner&gt;&lt;/div&gt;
                            <br/>&nbsp;&lt;/app-layout-auth&gt;
                        </code>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
</div>

<style>
    #documentação{ margin-top: -20px; margin-left: -50px; padding: 0px; width: calc(100% + 100px) }
    #documentação>div{ margin-bottom: 30px; background:rgba(225,255,255,0.1); padding: 20px 40px; }
    #documentação>div>h2{ margin-top: 0; }

    #documentação table { border-collapse: collapse; width:100%; }
    #documentação table td, #documentação table th { border: .5px solid #c0c0c0; padding: 10px 40px; }
    #documentação table thead { border-bottom: 2px solid #c0c0c0; text-transform: uppercase; }
    #documentação table thead th { font-weight: bold; text-align: center; background:#525252; color:white; font-size:120%; padding: 5px; }
    
    #documentação code{ padding:10px }
</style>
