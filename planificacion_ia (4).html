<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Leonardo Carrasco Ocon | Sistema IA de Planificación de Operaciones</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jszip/3.10.1/jszip.min.js"></script>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: 'Inter', sans-serif;
            background: #0a0e12;
            color: #eef2ff;
            line-height: 1.5;
        }
        .container { max-width: 1400px; margin: 0 auto; padding: 2rem 1.5rem; }
        .hero {
            background: linear-gradient(135deg, #0f212e 0%, #1a2f3c 100%);
            border-radius: 2rem;
            padding: 2rem;
            margin-bottom: 2rem;
            border: 1px solid rgba(0,255,255,0.2);
        }
        .hero h1 {
            font-size: 2rem;
            background: linear-gradient(135deg, #fff, #00f2fe);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        .autor {
            background: rgba(0,200,200,0.15);
            border-left: 3px solid #00f2fe;
            padding: 0.5rem 1rem;
            border-radius: 0.5rem;
            margin-top: 1rem;
        }
        .tabs-wrapper {
            margin-bottom: 1.5rem;
        }
        .tabs-grupo-label {
            font-size: 0.65rem;
            text-transform: uppercase;
            color: #5f8ca3;
            letter-spacing: 0.08em;
            margin-bottom: 0.3rem;
            margin-top: 0.8rem;
        }
        .tabs {
            display: flex;
            flex-wrap: wrap;
            gap: 0.4rem;
            padding-bottom: 0.4rem;
            border-bottom: 1px solid #1f3a44;
        }
        .tab-btn {
            background: #11181c;
            border: 1px solid #1f3a44;
            padding: 0.45rem 0.9rem;
            border-radius: 2rem;
            cursor: pointer;
            font-weight: 600;
            font-size: 0.82rem;
            transition: all 0.2s;
            white-space: nowrap;
        }
        .tab-btn:hover { background: #1f3a44; }
        .tab-btn.active {
            background: linear-gradient(135deg, #00f2fe, #4facfe);
            color: #0a0e12;
            border-color: transparent;
        }
        .tab-btn.grupo-mrp2 { border-color: #5b4ea8; }
        .tab-btn.grupo-mrp2.active { background: linear-gradient(135deg,#7c6fd4,#a78bfa); }
        .tab-btn.grupo-extra { border-color: #883c2c; }
        .tab-btn.grupo-extra.active { background: linear-gradient(135deg,#c05c3e,#f87171); }
        .tab-panel { display: none; }
        .tab-panel.active { display: block; }
        .card {
            background: #11181c;
            border-radius: 1.5rem;
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            border: 1px solid #1f3a44;
        }
        .card-title {
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: #00f2fe;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        .grid-2 { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 1rem; }
        .grid-3 { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem; }
        input, select {
            background: #0f1a1f;
            border: 1px solid #2a4b5c;
            padding: 0.6rem 1rem;
            border-radius: 0.8rem;
            color: white;
            width: 100%;
        }
        input:focus, select:focus { outline: none; border-color: #00f2fe; }
        label { font-size: 0.75rem; text-transform: uppercase; color: #8bb3cc; margin-bottom: 0.2rem; display: block; }
        button {
            background: #1f6d7a;
            border: none;
            padding: 0.6rem 1.2rem;
            border-radius: 2rem;
            color: white;
            font-weight: 600;
            cursor: pointer;
            margin-top: 0.5rem;
        }
        button:hover { background: #2aa3b3; transform: translateY(-2px); }
        .btn-excel {
            background: #1a5c2a;
            margin-left: 0.5rem;
        }
        .btn-excel:hover { background: #22793a; }
        .result-box {
            background: #0b1419;
            border-radius: 1rem;
            padding: 1rem;
            margin-top: 1rem;
            overflow-x: auto;
            font-size: 0.85rem;
            border: 1px solid #234a57;
        }
        .ia-insight {
            background: linear-gradient(135deg, #0e2a33, #0a1a1f);
            border-left: 4px solid #00f2fe;
            padding: 0.8rem;
            margin-top: 0.8rem;
            border-radius: 0.5rem;
            font-style: italic;
        }
        .warning { border-left-color: #facc15; background: #1f2a1a; }
        .success { border-left-color: #4ade80; background: #0a1f0a; }
        .danger { border-left-color: #f87171; background: #2a0f0f; }
        table { width: 100%; border-collapse: collapse; font-size: 0.8rem; }
        th, td { padding: 0.4rem; border-bottom: 1px solid #2a4b5c; text-align: center; }
        th { background: #10323e; color: #a5f3fc; }
        footer { text-align: center; margin-top: 2rem; padding: 1rem; color: #5f8ca3; font-size: 0.8rem; }
        .chart-container { margin-top: 1rem; background: #0c191f; padding: 0.5rem; border-radius: 1rem; }
        .badge-ia { background: #00f2fe20; padding: 0.2rem 0.5rem; border-radius: 1rem; font-size: 0.7rem; }
        .btn-row { display: flex; flex-wrap: wrap; gap: 0.5rem; margin-top: 0.8rem; align-items: center; }
        .btn-eliminar-bom { background: #883c2c !important; padding: 0.25rem 0.6rem !important; margin: 0 !important; border-radius: 0.5rem !important; font-size: 0.75rem; }
        .btn-eliminar-bom:hover { background: #b04a35 !important; transform: none !important; }
        .btn-agregar-bom { background: #1a5c2a !important; padding: 0.25rem 0.8rem !important; margin: 0 !important; border-radius: 0.5rem !important; font-size: 0.75rem; }
        .btn-agregar-bom:hover { background: #22793a !important; transform: none !important; }
        #tblBOM td input { padding: 0.3rem 0.5rem; border-radius: 0.4rem; font-size: 0.78rem; }
        .bom-nuevo-row td { background: rgba(0,242,254,0.05); }
    </style>
</head>
<body>
<div class="container" id="reportContainer">
    <div class="hero">
        <h1><i class="fas fa-brain"></i> SISTEMA IA DE PLANIFICACIÓN DE OPERACIONES</h1>
        <p>Promedio Móvil · Suavizado Exponencial · Regresión · PAP · PMP · MRP · BOM · Ordenes de Aprovisionamiento</p>
        <div class="autor" style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:0.5rem">
            <span><i class="fas fa-user-graduate"></i> <strong>Leonardo Carrasco Ocon</strong> — Autor & Desarrollador | <span class="badge-ia"><i class="fas fa-microchip"></i> IA Integrada</span></span>
            <div style="display:flex;gap:0.5rem;align-items:center">
                <span id="sesionEstado" style="font-size:0.72rem;color:#8bb3cc"></span>
                <button id="btnGuardarSesion" style="background:#1a5c2a;margin:0;padding:0.4rem 0.9rem;font-size:0.78rem">
                    <i class="fas fa-save"></i> Guardar sesión
                </button>
                <button id="btnCargarSesion" style="background:#1f6d7a;margin:0;padding:0.4rem 0.9rem;font-size:0.78rem">
                    <i class="fas fa-folder-open"></i> Cargar sesión
                </button>
                <button id="btnBorrarSesion" style="background:#883c2c;margin:0;padding:0.4rem 0.9rem;font-size:0.78rem">
                    <i class="fas fa-trash"></i> Borrar
                </button>
            </div>
        </div>
    </div>

    <div class="tabs-wrapper">
        <div class="tabs-grupo-label">📊 Pronósticos & Planificación</div>
        <div class="tabs">
            <button class="tab-btn active" data-tab="tab1">📊 Promedio Móvil</button>
            <button class="tab-btn" data-tab="tab2">📈 Suavizado Exp.</button>
            <button class="tab-btn" data-tab="tab3">📐 Regresión</button>
            <button class="tab-btn" data-tab="tab4">🏭 PAP</button>
            <button class="tab-btn" data-tab="tab5">📋 PMP</button>
        </div>
        <div class="tabs-grupo-label" style="margin-top:0.5rem">📦 MRP — Materiales</div>
        <div class="tabs">
            <button class="tab-btn" data-tab="tab6">📦 Inventarios</button>
            <button class="tab-btn" data-tab="tab7">🔧 BOM</button>
            <button class="tab-btn" data-tab="tab8">⚙️ MRP</button>
            <button class="tab-btn" data-tab="tab9">📝 Órdenes</button>
        </div>
        <div class="tabs-grupo-label" style="margin-top:0.5rem">🏭 MRP II — Recursos & Control</div>
        <div class="tabs">
            <button class="tab-btn grupo-mrp2" data-tab="tab10">⚡ CRP</button>
            <button class="tab-btn grupo-mrp2" data-tab="tab11">🏭 Control Planta</button>
            <button class="tab-btn grupo-mrp2" data-tab="tab12">🛒 Compras</button>
            <button class="tab-btn grupo-mrp2" data-tab="tab13">💰 Financiero</button>
        </div>
        <div class="tabs-grupo-label" style="margin-top:0.5rem">📋 Reportes & Documentación</div>
        <div class="tabs" style="border-bottom:none">
            <button class="tab-btn grupo-extra" data-tab="tab14">🖥️ ERP</button>
            <button class="tab-btn grupo-extra" data-tab="tab15">📚 Respaldo</button>
            <button class="tab-btn grupo-extra" data-tab="tab0">🎯 Portada</button>
        </div>
        <div class="tabs-grupo-label" style="margin-top:0.5rem">📐 Modelos de Inventario</div>
        <div class="tabs" style="border-bottom:none">
            <button class="tab-btn" style="border-color:#00f2fe" data-tab="tab16">📐 EOQ & Indicadores</button>
        </div>
    </div>

    <!-- TAB 1: PROMEDIO MÓVIL -->
    <div id="tab1" class="tab-panel active">
        <div class="card">
            <div class="card-title"><i class="fas fa-chart-line"></i> Pronóstico: Promedio Móvil Simple</div>
            <div class="grid-2">
                <div>
                    <label>📅 Datos históricos (12 meses, separados por comas)</label>
                    <input type="text" id="datosPM" placeholder="Ej: 312,317,345,346,361,340 (separar con comas)">
                </div>
                <div>
                    <label>🔢 Períodos a promediar (k) - número entero positivo</label>
                    <input type="number" id="kPM" placeholder="Ej: 3" min="1" step="1">
                </div>
            </div>
            <div class="btn-row">
                <button id="btnPM"><i class="fas fa-calculator"></i> Calcular Pronóstico</button>
                <button class="btn-excel" id="btnExcelPM"><i class="fas fa-file-excel"></i> Exportar a Excel</button>
            </div>
            <div id="resultadoPM" class="result-box">📊 Resultados del pronóstico por promedio móvil</div>
            <div class="chart-container"><canvas id="chartPM"></canvas></div>
        </div>
    </div>

    <!-- TAB 2: SUAVIZADO EXPONENCIAL -->
    <div id="tab2" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-chart-line"></i> Pronóstico: Suavizado Exponencial</div>
            <div class="grid-2">
                <div>
                    <label>📅 Datos históricos (12 meses)</label>
                    <input type="text" id="datosSE" placeholder="Ej: 312,317,345,346,361,340 (separar con comas)">
                </div>
                <div>
                    <label>🎯 Alfa (α) - valor entre 0 y 1</label>
                    <input type="number" id="alfaSE" placeholder="Ej: 0.3" step="0.01" min="0.01" max="0.99">
                </div>
            </div>
            <div class="btn-row">
                <button id="btnSE"><i class="fas fa-calculator"></i> Calcular Suavizado</button>
                <button class="btn-excel" id="btnExcelSE"><i class="fas fa-file-excel"></i> Exportar a Excel</button>
            </div>
            <div id="resultadoSE" class="result-box">📊 Resultados del suavizado exponencial</div>
            <div class="chart-container"><canvas id="chartSE"></canvas></div>
        </div>
    </div>

    <!-- TAB 3: REGRESIÓN LINEAL -->
    <div id="tab3" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-chart-scatter"></i> Regresión Lineal</div>
            <div class="grid-2">
                <div>
                    <label>📅 Períodos (X): 1,2,3,...,n</label>
                    <label>📊 Demanda histórica (Y):</label>
                    <input type="text" id="datosReg" placeholder="Ej: 312,317,345,346,361,340 (separar con comas)">
                </div>
                <div id="resultadoReg" class="result-box">📐 Ecuación de regresión y coeficientes</div>
            </div>
            <div class="btn-row">
                <button id="btnReg"><i class="fas fa-chart-line"></i> Calcular Regresión</button>
                <button class="btn-excel" id="btnExcelReg"><i class="fas fa-file-excel"></i> Exportar a Excel</button>
            </div>
            <div class="chart-container"><canvas id="chartReg"></canvas></div>
        </div>
    </div>

    <!-- TAB 4: PAP -->
    <div id="tab4" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-chart-line"></i> Plan Agregado de Producción (PAP) — 4 Estrategias</div>
            <div class="grid-3">
                <div><label>Proyección demanda 12 meses (pares)</label><input type="text" id="demandaPAP" placeholder="Ej: 312,317,345,346,361,340,333,321,335,328,374,376"></div>
                <div><label>Inventario inicial (pares)</label><input type="number" id="invInicialPAP" placeholder="Ej: 90"></div>
                <div><label>Reserva seguridad (% demanda)</label><input type="number" id="rsPAP" placeholder="Ej: 20" step="1"></div>
                <div><label>Días laborables/mes</label><input type="number" id="diasLabPAP" placeholder="Ej: 22"></div>
                <div><label>Horas trabajo requeridas (hh/par)</label><input type="number" id="hhPAP" placeholder="Ej: 2" step="0.1"></div>
                <div><label>Jornada diaria (h/día)</label><input type="number" id="jornadaPAP" placeholder="Ej: 8"></div>
                <div><label>Costo lineal (S/./hora)</label><input type="number" id="costoHoraPAP" placeholder="Ej: 7.00"></div>
                <div><label>Costo tiempo extra (S/./hora)</label><input type="number" id="costoHoraExtraPAP" placeholder="Ej: 9.00"></div>
                <div><label>Costo mantener inventario (S/./par/mes)</label><input type="number" id="costoMantPAP" placeholder="Ej: 4.00"></div>
                <div><label>Costo agotamiento/faltante (S/./par/mes)</label><input type="number" id="costoFaltPAP" placeholder="Ej: 32.00"></div>
                <div><label>Costo subcontratación (S/./par)</label><input type="number" id="costoSubPAP" placeholder="Ej: 35.00"></div>
                <div><label>Costo contratación (S/./trabajador)</label><input type="number" id="costoContPAP" placeholder="Ej: 930"></div>
                <div><label>Costo despido (S/./trabajador)</label><input type="number" id="costoDesPAP" placeholder="Ej: 1000"></div>
            </div>
            <div class="btn-row">
                <button id="btnPAP"><i class="fas fa-calculator"></i> Calcular 4 Planes</button>
                <button class="btn-excel" id="btnExcelPAP"><i class="fas fa-file-excel"></i> Exportar a Excel</button>
            </div>
            <div id="resultadoPAP" class="result-box">📊 Resultados del Plan Agregado — 4 estrategias</div>
            <div class="chart-container"><canvas id="chartPAP"></canvas></div>
        </div>
    </div>

    <!-- TAB 5: PMP -->
    <div id="tab5" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-clipboard-list"></i> Plan Maestro de Producción (PMP)</div>
            <div class="grid-3">
                <div><label>Req. producción mes 1 — total agregado (pares)</label><input type="number" id="reqProdPAP" placeholder="Total pares a producir"></div>
                <div><label>Días laborables/mes</label><input type="number" id="diasLab" placeholder="Ej: 22"></div>
                <div><label>Capacidad planta normal (lotes/mes)</label><input type="number" id="capPlanta" placeholder="Ej: 26"></div>
                <div><label>Lote mínimo (pares/corrida)</label><input type="number" id="loteMin" placeholder="Ej: 14.18"></div>
            </div>
            <div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:0.5rem;margin:0.5rem 0">
                <p style="font-size:0.8rem;color:#8bb3cc;margin:0">SKUs — Se generan automáticamente desde los productos nivel 0 del BOM:</p>
                <button id="btnPMPdesdeBOM" style="background:#5b4ea8;margin:0;padding:0.35rem 0.9rem;font-size:0.78rem">
                    <i class="fas fa-sitemap"></i> Recargar desde BOM
                </button>
            </div>
            <div id="pmpSkusGrid" style="margin-top:0.5rem">
                <p style="color:#8bb3cc;font-size:0.8rem">Presiona "Recargar desde BOM" para generar los campos de cada SKU.</p>
            </div>
            <div class="btn-row">
                <button id="btnPMP"><i class="fas fa-calculator"></i> Calcular PMP</button>
                <button class="btn-excel" id="btnExcelPMP"><i class="fas fa-file-excel"></i> Exportar a Excel</button>
            </div>
            <div id="resultadoPMP" class="result-box">📋 Programa Maestro de Producción</div>
            <div class="chart-container"><canvas id="chartPMP"></canvas></div>
        </div>
    </div>

    <!-- TAB 6: INVENTARIOS -->
    <div id="tab6" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-boxes"></i> Inventario de Materiales</div>
            <div id="tablaInventarios" class="result-box">
                <table id="tblInventarios">
                    <thead><tr>
                        <th>Material</th><th>Und</th><th>Stock Inicial</th>
                        <th>Tamaño Lote</th><th>Lead Time (sem)</th><th>Acción</th>
                    </tr></thead>
                    <tbody></tbody>
                </table>
            </div>
            <div class="btn-row">
                <button id="btnAgregarInv" style="background:#1a5c2a"><i class="fas fa-plus"></i> Nueva fila</button>
                <button id="btnGuardarInv"><i class="fas fa-save"></i> Guardar Cambios</button>
                <button class="btn-excel" id="btnExcelInv"><i class="fas fa-file-excel"></i> Exportar a Excel</button>
            </div>
        </div>
    </div>

    <!-- TAB 7: BOM (EDITABLE) -->
    <div id="tab7" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-sitemap"></i> Lista de Materiales (BOM) — <span id="bomEstado" style="font-size:0.8rem; font-weight:400; color:#8bb3cc;">Modo Lectura</span></div>
            <div id="tablaBOM" class="result-box">
                <table id="tblBOM">
                    <thead><tr><th>Producto/Componente</th><th>Nivel</th><th>Componente</th><th>Cantidad</th><th>Unidad</th></tr></thead>
                    <tbody></tbody>
                </table>
            </div>
            <div class="btn-row">
                <button id="btnEditarBOM" style="background:#1f6d7a;"><i class="fas fa-edit"></i> Editar BOM</button>
                <button id="btnGuardarBOM" style="background:#1a5c2a; display:none;"><i class="fas fa-save"></i> Guardar BOM</button>
                <button class="btn-excel" id="btnExcelBOM"><i class="fas fa-file-excel"></i> Exportar a Excel</button>
            </div>
        </div>
    </div>

    <datalist id="undList">
        <option value="Litro"><option value="Galón"><option value="Metro">
        <option value="Pie2"><option value="Par"><option value="Unidad">
        <option value="Cono"><option value="Plancha"><option value="Kg">
        <option value="Doc"><option value="Pza"><option value="Batch">
        <option value="Rollo"><option value="Caja"><option value="Bolsa">
    </datalist>
    <!-- TAB 8: MRP -->
    <div id="tab8" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-microchip"></i> Material Requirements Planning (MRP)</div>

            <!-- Configuración principal -->
            <div class="grid-3" style="margin-bottom:0.8rem">
                <div>
                    <label>Seleccionar material</label>
                    <select id="materialMRP" onchange="actualizarMaterialMRP()">
                        <!-- Se llena dinámicamente desde inventariosData -->
                    </select>
                </div>
                <div>
                    <label>Modo de planificación</label>
                    <select id="modoMRP" onchange="generarInputsMRP()">
                        <option value="semanas">Semanas (hasta 52)</option>
                        <option value="meses">Meses (hasta 12)</option>
                    </select>
                </div>
                <div>
                    <label>Número de períodos a planificar</label>
                    <input type="number" id="nPeriodosMRP" value="8" min="1" max="52"
                           placeholder="Ej: 8" onchange="generarInputsMRP()">
                </div>
                <div>
                    <label>Períodos previos con stock (contexto LT)</label>
                    <input type="number" id="periodosPrevMRP" value="0" min="0" max="12"
                           placeholder="Ej: 4" onchange="generarInputsMRP()">
                </div>
                <div id="infoMaterialMRP" style="background:#0f1a1f;border:1px solid #2a4b5c;border-radius:0.8rem;padding:0.6rem;font-size:0.78rem;color:#8bb3cc">
                    Selecciona un material para ver su información
                </div>
            </div>

            <!-- Tabla de NB dinámica -->
            <div id="contenedorNBMRP" class="result-box" style="margin-bottom:0.8rem">
                <p style="color:#8bb3cc;font-size:0.8rem">Configura los parámetros y se generarán los campos de Necesidades Brutas automáticamente.</p>
            </div>

            <div class="btn-row">
                <button id="btnMRP"><i class="fas fa-cogs"></i> Calcular MRP</button>
                <button id="btnAgregarOrden" style="background:#1a5c2a;display:none"><i class="fas fa-plus-circle"></i> Agregar a Órdenes</button>
                <button id="btnSyncMRP" style="background:#5b4ea8"><i class="fas fa-sync-alt"></i> Actualizar materiales</button>
                <button id="btnLimpiarMRP" style="background:#883c2c"><i class="fas fa-eraser"></i> Limpiar NB</button>
                <button class="btn-excel" id="btnExcelMRP"><i class="fas fa-file-excel"></i> Exportar a Excel</button>
            </div>
            <div id="resultadoMRP" class="result-box">⚙️ Configura los parámetros y presiona Calcular MRP</div>
            <div class="chart-container"><canvas id="chartMRP"></canvas></div>
        </div>
    </div>

    <!-- TAB 9: ÓRDENES -->
    <div id="tab9" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-truck"></i> Ordenes de Aprovisionamiento</div>
            <div id="resultadoOrdenes" class="result-box">📋 Programa de ordenes de compra y producción</div>
            <div class="btn-row">
                <button id="btnExportarOrdenes"><i class="fas fa-file-excel"></i> Exportar a CSV</button>
                <button class="btn-excel" id="btnExcelOrdenes"><i class="fas fa-file-excel"></i> Exportar a Excel</button>
                <button id="btnExportarPDF" style="background: #883c2c;"><i class="fas fa-file-pdf"></i> Exportar todo a PDF</button>
            </div>
        </div>
    </div>


    <!-- TAB 10: CRP -->
    <div id="tab10" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-tachometer-alt"></i> CRP — Capacity Requirements Planning</div>
            <p style="font-size:0.8rem;color:#8bb3cc;margin-bottom:0.8rem">Verifica si la capacidad disponible cubre los requerimientos del MRP. Se alimenta del PAP y MRP calculados.</p>
            <div class="grid-3">
                <div><label>Centros de trabajo (separados por coma)</label><input type="text" id="crpCentros" placeholder="Ej: Corte,Costura,Montaje,Acabado"></div>
                <div><label>Capacidad disponible por centro (h/sem, comas)</label><input type="text" id="crpCapDisp" placeholder="Ej: 176,176,176,176"></div>
                <div><label>Horas requeridas por centro por par (comas)</label><input type="text" id="crpHhCentro" placeholder="Ej: 0.5,0.8,0.4,0.3"></div>
                <div><label>Eficiencia por centro % (comas)</label><input type="text" id="crpEfic" placeholder="Ej: 90,85,92,88"></div>
                <div><label>Semanas a planificar</label><input type="number" id="crpSemanas" placeholder="Ej: 4" min="1" max="52"></div>
                <div><label>Producción semanal (pares, desde MRP o manual)</label><input type="text" id="crpProdSem" placeholder="Ej: 88,88,88,88"></div>
            </div>
            <div class="btn-row">
                <button id="btnCRP"><i class="fas fa-calculator"></i> Calcular CRP</button>
                <button id="btnCRPdesdeMRP" style="background:#5b4ea8"><i class="fas fa-sync-alt"></i> Cargar desde MRP</button>
                <button class="btn-excel" id="btnExcelCRP"><i class="fas fa-file-excel"></i> Exportar Excel</button>
            </div>
            <div id="resultadoCRP" class="result-box">⚡ Resultados de Capacidad por Centro de Trabajo</div>
            <div class="chart-container"><canvas id="chartCRP"></canvas></div>
        </div>
    </div>

    <!-- TAB 11: CONTROL DE PLANTA -->
    <div id="tab11" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-industry"></i> Control de Planta — Shop Floor Control</div>
            <p style="font-size:0.8rem;color:#8bb3cc;margin-bottom:0.8rem">Seguimiento de órdenes de producción: eficiencia real vs planificada, avance por semana.</p>
            <div class="grid-3">
                <div><label>Producción planificada/semana (pares)</label><input type="text" id="sfcPlanif" placeholder="Ej: 88,88,88,88"></div>
                <div><label>Producción real/semana (pares)</label><input type="text" id="sfcReal" placeholder="Ej: 82,90,85,79"></div>
                <div><label>Horas planificadas/semana</label><input type="text" id="sfcHPlan" placeholder="Ej: 176,176,176,176"></div>
                <div><label>Horas reales utilizadas/semana</label><input type="text" id="sfcHReal" placeholder="Ej: 168,180,172,165"></div>
                <div><label>Costo mano de obra planificado/semana (S/.)</label><input type="text" id="sfcCostoPlan" placeholder="Ej: 1232,1232,1232,1232"></div>
                <div><label>Costo mano de obra real/semana (S/.)</label><input type="text" id="sfcCostoReal" placeholder="Ej: 1176,1260,1204,1155"></div>
            </div>
            <div class="btn-row">
                <button id="btnSFC"><i class="fas fa-calculator"></i> Calcular Control Planta</button>
                <button class="btn-excel" id="btnExcelSFC"><i class="fas fa-file-excel"></i> Exportar Excel</button>
            </div>
            <div id="resultadoSFC" class="result-box">🏭 Resultados de Control de Planta</div>
            <div class="chart-container"><canvas id="chartSFC"></canvas></div>
        </div>
    </div>

    <!-- TAB 12: COMPRAS -->
    <div id="tab12" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-shopping-cart"></i> Gestión de Compras y Proveedores</div>
            <p style="font-size:0.8rem;color:#8bb3cc;margin-bottom:0.8rem">Órdenes de compra automáticas desde el MRP, con seguimiento de proveedores y fechas de entrega.</p>
            <div id="tablaCompras" class="result-box">
                <table id="tblCompras">
                    <thead><tr>
                        <th>Material</th><th>Proveedor</th><th>Cantidad</th><th>Precio Unit. (S/.)</th>
                        <th>Total (S/.)</th><th>Fecha Pedido</th><th>Fecha Entrega</th><th>Estado</th>
                    </tr></thead>
                    <tbody id="tbodyCompras"></tbody>
                </table>
            </div>
            <div class="btn-row">
                <button id="btnGenerarCompras" style="background:#1a5c2a"><i class="fas fa-magic"></i> Generar desde MRP</button>
                <button id="btnAgregarCompra" style="background:#1f6d7a"><i class="fas fa-plus"></i> Agregar Fila</button>
                <button class="btn-excel" id="btnExcelCompras"><i class="fas fa-file-excel"></i> Exportar Excel</button>
            </div>
        </div>
    </div>

    <!-- TAB 13: PLANIFICACIÓN FINANCIERA -->
    <div id="tab13" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-dollar-sign"></i> Planificación Financiera MRP II</div>
            <p style="font-size:0.8rem;color:#8bb3cc;margin-bottom:0.8rem">Traduce el plan de producción a costos, presupuesto y flujo de caja mensual.</p>
            <div class="grid-3">
                <div><label>Precio de venta por par (S/.)</label><input type="number" id="finPrecioVenta" placeholder="Ej: 85"></div>
                <div><label>Costo materia prima por par (S/.)</label><input type="number" id="finCostoMP" placeholder="Ej: 28"></div>
                <div><label>Costo mano de obra por par (S/.)</label><input type="number" id="finCostoMO" placeholder="Ej: 14"></div>
                <div><label>Costos indirectos fab. por par (S/.)</label><input type="number" id="finCIF" placeholder="Ej: 8"></div>
                <div><label>Gastos administración/mes (S/.)</label><input type="number" id="finGastosAdmin" placeholder="Ej: 2500"></div>
                <div><label>Gastos ventas/mes (S/.)</label><input type="number" id="finGastosVentas" placeholder="Ej: 1800"></div>
            </div>
            <div class="btn-row">
                <button id="btnFinanciero"><i class="fas fa-calculator"></i> Calcular Plan Financiero</button>
                <button id="btnFinDesdePAP" style="background:#5b4ea8"><i class="fas fa-sync-alt"></i> Cargar desde PAP/PMP</button>
                <button class="btn-excel" id="btnExcelFinanciero"><i class="fas fa-file-excel"></i> Exportar Excel</button>
            </div>
            <div id="resultadoFinanciero" class="result-box">💰 Plan Financiero — Ingresos, Costos y Flujo de Caja</div>
            <div class="chart-container"><canvas id="chartFinanciero"></canvas></div>
        </div>
    </div>

    <!-- TAB 14: ERP SIMULADO -->
    <div id="tab14" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-server"></i> Simulación ERP — Pantallas Tipo SAP/Odoo</div>
            <p style="font-size:0.8rem;color:#8bb3cc;margin-bottom:0.8rem">
                Visualización de los datos del sistema en formato ERP. Genera capturas exportables para tu informe.
            </p>
            <div class="btn-row" style="margin-bottom:1rem">
                <button id="btnERPActualizar" style="background:#1a5c2a"><i class="fas fa-sync-alt"></i> Actualizar pantallas ERP</button>
                <button id="btnERPCaptura" style="background:#883c2c"><i class="fas fa-camera"></i> Capturar como imagen</button>
            </div>

            <!-- Pantalla ERP 1: Cabecera tipo SAP -->
            <div id="erpContainer" style="font-family:monospace;background:#f5f5f0;color:#222;border-radius:0.5rem;overflow:hidden;border:2px solid #ccc">

                <!-- Barra de menú ERP -->
                <div style="background:#0a3055;color:white;padding:6px 12px;display:flex;align-items:center;gap:12px;font-size:0.8rem">
                    <span style="font-weight:700;font-size:1rem;color:#7ec8e3">▣ ERP-MRP II</span>
                    <span style="opacity:0.7">Sistema de Planificación de Recursos de Manufactura</span>
                    <span style="margin-left:auto;opacity:0.7" id="erpFechaHora"></span>
                </div>

                <!-- Barra de transacción tipo SAP -->
                <div style="background:#e8e8dc;border-bottom:1px solid #bbb;padding:4px 12px;display:flex;gap:16px;font-size:0.75rem">
                    <span>📁 Logística</span><span>▶</span>
                    <span>Producción</span><span>▶</span>
                    <span>Planificación de Necesidades</span><span>▶</span>
                    <span style="font-weight:700">Evaluación MRP</span>
                </div>

                <div style="padding:12px;display:grid;grid-template-columns:1fr 1fr;gap:12px">

                    <!-- Módulo 1: Órdenes planificadas MRP -->
                    <div style="background:white;border:1px solid #bbb;border-radius:4px;overflow:hidden">
                        <div style="background:#0a3055;color:white;padding:5px 10px;font-size:0.75rem;font-weight:700">
                            📋 MD04 — Lista de Necesidades/Stock
                        </div>
                        <div style="padding:8px" id="erpMD04">
                            <div style="color:#888;font-size:0.72rem">Ejecuta el MRP para ver datos</div>
                        </div>
                    </div>

                    <!-- Módulo 2: PAP / Plan de producción -->
                    <div style="background:white;border:1px solid #bbb;border-radius:4px;overflow:hidden">
                        <div style="background:#0a3055;color:white;padding:5px 10px;font-size:0.75rem;font-weight:700">
                            🏭 MC87 — Plan Agregado de Producción
                        </div>
                        <div style="padding:8px" id="erpMC87">
                            <div style="color:#888;font-size:0.72rem">Ejecuta el PAP para ver datos</div>
                        </div>
                    </div>

                    <!-- Módulo 3: Lista de materiales BOM -->
                    <div style="background:white;border:1px solid #bbb;border-radius:4px;overflow:hidden">
                        <div style="background:#0a3055;color:white;padding:5px 10px;font-size:0.75rem;font-weight:700">
                            🔧 CS03 — Lista de Materiales (BOM)
                        </div>
                        <div style="padding:8px;max-height:200px;overflow-y:auto" id="erpCS03">
                            <div style="color:#888;font-size:0.72rem">Cargando BOM...</div>
                        </div>
                    </div>

                    <!-- Módulo 4: Inventario / Stock -->
                    <div style="background:white;border:1px solid #bbb;border-radius:4px;overflow:hidden">
                        <div style="background:#0a3055;color:white;padding:5px 10px;font-size:0.75rem;font-weight:700">
                            📦 MMBE — Vista General de Stock
                        </div>
                        <div style="padding:8px;max-height:200px;overflow-y:auto" id="erpMMBE">
                            <div style="color:#888;font-size:0.72rem">Cargando inventario...</div>
                        </div>
                    </div>

                    <!-- Módulo 5: CRP / Capacidad -->
                    <div style="background:white;border:1px solid #bbb;border-radius:4px;overflow:hidden">
                        <div style="background:#0a3055;color:white;padding:5px 10px;font-size:0.75rem;font-weight:700">
                            ⚡ CM01 — Perfil de Capacidad (CRP)
                        </div>
                        <div style="padding:8px" id="erpCM01">
                            <div style="color:#888;font-size:0.72rem">Ejecuta el CRP para ver datos</div>
                        </div>
                    </div>

                    <!-- Módulo 6: Órdenes de compra -->
                    <div style="background:white;border:1px solid #bbb;border-radius:4px;overflow:hidden">
                        <div style="background:#0a3055;color:white;padding:5px 10px;font-size:0.75rem;font-weight:700">
                            🛒 ME2M — Órdenes de Compra por Material
                        </div>
                        <div style="padding:8px;max-height:200px;overflow-y:auto" id="erpME2M">
                            <div style="color:#888;font-size:0.72rem">Ejecuta Compras para ver datos</div>
                        </div>
                    </div>
                </div>

                <!-- Barra de estado tipo SAP -->
                <div style="background:#e8e8dc;border-top:1px solid #bbb;padding:3px 12px;font-size:0.7rem;color:#555;display:flex;justify-content:space-between">
                    <span id="erpStatus">Sistema listo</span>
                    <span>Leonardo Carrasco Ocon | MRP II v2.0 | © 2026</span>
                </div>
            </div>
        </div>
    </div>

    <!-- TAB 15: MATERIAL DE RESPALDO -->
    <div id="tab15" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-book"></i> Material de Respaldo — Glosario, Fórmulas y Bibliografía</div>

            <!-- Glosario -->
            <div style="margin-bottom:1.5rem">
                <p style="font-weight:700;color:#00f2fe;margin-bottom:0.5rem"><i class="fas fa-list"></i> Glosario de Términos MRP / MRP II</p>
                <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:0.5rem" id="glosario"></div>
            </div>

            <!-- Fórmulas -->
            <div style="margin-bottom:1.5rem">
                <p style="font-weight:700;color:#00f2fe;margin-bottom:0.5rem"><i class="fas fa-square-root-alt"></i> Fórmulas Utilizadas en el Sistema</p>
                <div id="formulasRespaldo"></div>
            </div>

            <!-- Bibliografía -->
            <div>
                <p style="font-weight:700;color:#00f2fe;margin-bottom:0.5rem"><i class="fas fa-book-open"></i> Bibliografía de Referencia</p>
                <div id="bibliografiaRespaldo"></div>
            </div>

            <div class="btn-row" style="margin-top:1rem">
                <button id="btnExportarRespaldo" style="background:#883c2c"><i class="fas fa-file-pdf"></i> Exportar Material a PDF</button>
            </div>
        </div>
    </div>

    <!-- TAB 0: PORTADA -->
    <div id="tab0" class="tab-panel">
        <div id="portadaContainer">
            <div style="background:linear-gradient(135deg,#0f212e,#1a2f3c);border-radius:2rem;padding:3rem;border:1px solid rgba(0,255,255,0.3);text-align:center;margin-bottom:1.5rem">
                <div style="font-size:3rem;margin-bottom:0.5rem">🏭</div>
                <h1 style="font-size:2.2rem;background:linear-gradient(135deg,#fff,#00f2fe);-webkit-background-clip:text;background-clip:text;color:transparent;margin-bottom:0.5rem">
                    SISTEMA MRP II
                </h1>
                <h2 style="font-size:1.2rem;color:#8bb3cc;font-weight:400;margin-bottom:1.5rem">
                    Manufacturing Resource Planning — Planificación de Recursos de Manufactura
                </h2>
                <div style="width:80px;height:3px;background:linear-gradient(135deg,#00f2fe,#4facfe);margin:0 auto 2rem"></div>

                <!-- Datos editables de la portada -->
                <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:1rem;max-width:800px;margin:0 auto 2rem;text-align:left">
                    <div>
                        <label style="font-size:0.7rem;color:#8bb3cc;text-transform:uppercase">Autor</label>
                        <input type="text" id="portadaAutor" value="Leonardo Carrasco Ocon" style="background:rgba(0,242,254,0.1);border:1px solid rgba(0,242,254,0.3);border-radius:0.5rem;padding:0.5rem;color:white;width:100%;text-align:center">
                    </div>
                    <div>
                        <label style="font-size:0.7rem;color:#8bb3cc;text-transform:uppercase">Empresa / Institución</label>
                        <input type="text" id="portadaEmpresa" placeholder="Nombre de la empresa" style="background:rgba(0,242,254,0.1);border:1px solid rgba(0,242,254,0.3);border-radius:0.5rem;padding:0.5rem;color:white;width:100%;text-align:center">
                    </div>
                    <div>
                        <label style="font-size:0.7rem;color:#8bb3cc;text-transform:uppercase">Curso / Materia</label>
                        <input type="text" id="portadaCurso" placeholder="Ej: Gestión de Operaciones" style="background:rgba(0,242,254,0.1);border:1px solid rgba(0,242,254,0.3);border-radius:0.5rem;padding:0.5rem;color:white;width:100%;text-align:center">
                    </div>
                    <div>
                        <label style="font-size:0.7rem;color:#8bb3cc;text-transform:uppercase">Profesor / Asesor</label>
                        <input type="text" id="portadaProfesor" placeholder="Nombre del profesor" style="background:rgba(0,242,254,0.1);border:1px solid rgba(0,242,254,0.3);border-radius:0.5rem;padding:0.5rem;color:white;width:100%;text-align:center">
                    </div>
                    <div>
                        <label style="font-size:0.7rem;color:#8bb3cc;text-transform:uppercase">Período</label>
                        <input type="text" id="portadaPeriodo" placeholder="Ej: 2026-I" style="background:rgba(0,242,254,0.1);border:1px solid rgba(0,242,254,0.3);border-radius:0.5rem;padding:0.5rem;color:white;width:100%;text-align:center">
                    </div>
                    <div>
                        <label style="font-size:0.7rem;color:#8bb3cc;text-transform:uppercase">Fecha</label>
                        <input type="text" id="portadaFecha" style="background:rgba(0,242,254,0.1);border:1px solid rgba(0,242,254,0.3);border-radius:0.5rem;padding:0.5rem;color:white;width:100%;text-align:center">
                    </div>
                </div>

                <!-- Módulos del sistema -->
                <div style="max-width:700px;margin:0 auto">
                    <p style="font-size:0.8rem;color:#8bb3cc;margin-bottom:1rem">MÓDULOS DEL SISTEMA</p>
                    <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:0.5rem">
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">📊</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">Pronósticos</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">PM · SE · Regresión</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">🏭</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">PAP</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">4 Estrategias de Producción</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">📋</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">PMP</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Plan Maestro 4 SKUs</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">📦</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">Inventarios & BOM</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Gestión de Materiales</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">⚙️</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">MRP</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Semanas / Meses</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">📝</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">Órdenes</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Aprovisionamiento</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">⚡</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">CRP</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Capacidad por Centro</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">🏭</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">Control Planta</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Real vs Planificado</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">🛒</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">Compras</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Gestión Proveedores</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">💰</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">Financiero</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Ingresos & Utilidad</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">🖥️</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">ERP Simulado</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Pantallas Tipo SAP</div>
                        </div>
                        <div style="background:rgba(0,242,254,0.05);border:1px solid rgba(0,242,254,0.15);border-radius:0.8rem;padding:0.7rem">
                            <div style="font-size:1.3rem">📚</div>
                            <div style="font-weight:600;font-size:0.8rem;color:#00f2fe">Respaldo</div>
                            <div style="font-size:0.65rem;color:#8bb3cc">Glosario · Fórmulas · Biblio</div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="btn-row" style="justify-content:center">
                <button id="btnPortadaPDF" style="background:#883c2c;font-size:1rem;padding:0.8rem 2rem"><i class="fas fa-file-pdf"></i> Exportar Portada a PDF</button>
            </div>
        </div>
    </div>

    <!-- TAB 16: EOQ & INDICADORES -->
    <div id="tab16" class="tab-panel">
        <div class="card">
            <div class="card-title"><i class="fas fa-calculator"></i> EOQ, ROP e Indicadores de Inventario</div>

            <!-- EOQ -->
            <p style="font-weight:700;color:#00f2fe;margin-bottom:0.5rem">📐 EOQ — Cantidad Económica de Pedido</p>
            <div class="grid-3">
                <div><label>Material (referencia)</label>
                    <select id="eoqMaterial" onchange="autocompletarEOQ()">
                        <option value="">— Seleccionar —</option>
                    </select>
                </div>
                <div><label>Demanda anual (D) — unidades/año</label>
                    <input type="number" id="eoqD" placeholder="Ej: 5000" step="any"></div>
                <div><label>Costo por pedido (S) — S/./orden</label>
                    <input type="number" id="eoqS" placeholder="Ej: 50" step="any"></div>
                <div><label>Costo unitario (C) — S/./unidad</label>
                    <input type="number" id="eoqC" placeholder="Ej: 12" step="any"></div>
                <div><label>Tasa mantenimiento anual (i) — %</label>
                    <input type="number" id="eoqI" placeholder="Ej: 25" step="any"></div>
                <div><label>Lead Time (L) — días</label>
                    <input type="number" id="eoqL" placeholder="Ej: 14" step="any"></div>
                <div><label>Días laborables/año</label>
                    <input type="number" id="eoqDias" placeholder="Ej: 264" value="264"></div>
                <div><label>Stock de seguridad (SS) — unidades</label>
                    <input type="number" id="eoqSS" placeholder="Ej: 50" step="any"></div>
                <div><label>Nivel de servicio objetivo (%)</label>
                    <input type="number" id="eoqNS" placeholder="Ej: 95" step="any" value="95"></div>
            </div>
            <div class="btn-row">
                <button id="btnEOQ"><i class="fas fa-calculator"></i> Calcular EOQ</button>
                <button id="btnEOQdesdeMRP" style="background:#5b4ea8"><i class="fas fa-sync-alt"></i> Cargar desde MRP</button>
                <button id="btnEnviarROP" style="background:#1a5c2a"><i class="fas fa-paper-plane"></i> Enviar ROP al MRP</button>
                <button class="btn-excel" id="btnExcelEOQ"><i class="fas fa-file-excel"></i> Exportar Excel</button>
            </div>
            <div id="resultadoEOQ" class="result-box">📐 Resultados EOQ aparecerán aquí</div>
            <div class="chart-container"><canvas id="chartEOQ"></canvas></div>
        </div>

        <!-- Indicadores -->
        <div class="card" style="margin-top:1rem">
            <div class="card-title"><i class="fas fa-tachometer-alt"></i> Indicadores de Inventario — Panel de Control</div>
            <p style="font-size:0.8rem;color:#8bb3cc;margin-bottom:0.8rem">Se calculan automáticamente desde los datos del MRP, PAP y EOQ.</p>
            <div class="btn-row" style="margin-bottom:0.8rem">
                <button id="btnIndicadores"><i class="fas fa-sync-alt"></i> Calcular Indicadores</button>
            </div>
            <div id="resultadoIndicadores" class="result-box">
                <p style="color:#8bb3cc;font-size:0.85rem">Presiona "Calcular Indicadores" para ver el panel completo.</p>
            </div>
            <div class="chart-container"><canvas id="chartIndicadores"></canvas></div>
        </div>
    </div>
    <footer>© 2026 Leonardo Carrasco Ocon — Sistema MRP II Integral | IA Integrada</footer>
</div>

<script>
    // ================= DATOS POR DEFECTO =================
    const inventariosData = [
        { material: "SKU1 - Ballerina Talla 37 Negro", und: "Doc", stock: 0, lote: "LFL", lt: 0 },
        { material: "SKU2 - Ballerina Talla 38 Marrón", und: "Doc", stock: 0, lote: "LFL", lt: 0 },
        { material: "SKU3 - Sandalia Baja Talla 37 Negro", und: "Doc", stock: 0, lote: "LFL", lt: 0 },
        { material: "SKU4 - Sandalia Baja Talla 38 Marrón", und: "Doc", stock: 0, lote: "LFL", lt: 0 },
        { material: "Zapato Ballerina - 1 Talla 37", und: "Batch", stock: 0, lote: "LFL", lt: 0 },
        { material: "Zapato Ballerina - 2 Talla 38", und: "Batch", stock: 0, lote: "LFL", lt: 0 },
        { material: "Cuero Charol Negro", und: "Pie2", stock: 700, lote: 500, lt: 3 },
        { material: "Cuero Blanco", und: "Pie2", stock: 500, lote: 700, lt: 3 },
        { material: "Bolsa de despacho", und: "Pza", stock: 1000, lote: 1500, lt: 1 },
        { material: "Caja de empaque", und: "Pza", stock: 1000, lote: 500, lt: 1 },
        { material: "Etiqueta de marca", und: "Pza", stock: 100, lote: 150, lt: 1 },
        { material: "Pegamento Hot melt", und: "Pza", stock: 30, lote: 35, lt: 3 }
    ];

    let bomData = [
        // ── SKU 1: cód. 476 cerrado vestir ──────────────────────────
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 0, comp: "Producto Final",   cant: 1,      und: "Par" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Bencina",           cant: 0.0167, und: "Litro" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Tintes",            cant: 0.0218, und: "Litro" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Deslizador Horma",  cant: 0.0042, und: "Litro" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Suela",             cant: 1,      und: "Par" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Ceras",             cant: 0.0111, und: "Unidad" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Bolsa Transparente",cant: 1,      und: "Unidad" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Caja Tipo A",       cant: 1,      und: "Unidad" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Falsas",            cant: 1,      und: "Par" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Tacos",             cant: 1,      und: "Par" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Plantilla A",       cant: 1,      und: "Par" },
        { prod: "SKU1 - cód.476 cerrado vestir", nivel: 1, comp: "Pieza Aparada 1",   cant: 1,      und: "Par" },

        // ── SKU 2: cód. 579 botín sport ─────────────────────────────
        { prod: "SKU2 - cód.579 botín sport",    nivel: 0, comp: "Producto Final",   cant: 1,      und: "Par" },
        { prod: "SKU2 - cód.579 botín sport",    nivel: 1, comp: "Bencina",           cant: 0.0167, und: "Litro" },
        { prod: "SKU2 - cód.579 botín sport",    nivel: 1, comp: "Tintes",            cant: 0.0038, und: "Litro" },
        { prod: "SKU2 - cód.579 botín sport",    nivel: 1, comp: "Planta",            cant: 2,      und: "Unidad" },
        { prod: "SKU2 - cód.579 botín sport",    nivel: 1, comp: "Bolsa Transparente",cant: 1,      und: "Unidad" },
        { prod: "SKU2 - cód.579 botín sport",    nivel: 1, comp: "Caja Tipo B",       cant: 1,      und: "Unidad" },
        { prod: "SKU2 - cód.579 botín sport",    nivel: 1, comp: "Falsas",            cant: 1,      und: "Par" },
        { prod: "SKU2 - cód.579 botín sport",    nivel: 1, comp: "Plantilla B",       cant: 1,      und: "Par" },
        { prod: "SKU2 - cód.579 botín sport",    nivel: 1, comp: "Pieza Aparada 5",   cant: 1,      und: "Par" },

        // ── COMP 1.1: Pieza Aparada 1 ────────────────────────────────
        { prod: "COMP1.1 - Pieza Aparada 1",     nivel: 2, comp: "Hilos",             cant: 0.0133, und: "Cono" },
        { prod: "COMP1.1 - Pieza Aparada 1",     nivel: 2, comp: "Cuero",             cant: 1.5,    und: "Pie2" },
        { prod: "COMP1.1 - Pieza Aparada 1",     nivel: 2, comp: "Badana",            cant: 1.4333, und: "Pie2" },
        { prod: "COMP1.1 - Pieza Aparada 1",     nivel: 2, comp: "Lona",              cant: 0.0167, und: "Metro" },
        { prod: "COMP1.1 - Pieza Aparada 1",     nivel: 2, comp: "Contrafuertes",     cant: 0.0194, und: "Plancha" },
        { prod: "COMP1.1 - Pieza Aparada 1",     nivel: 2, comp: "Cintillo",          cant: 0.0167, und: "Cono" },
        { prod: "COMP1.1 - Pieza Aparada 1",     nivel: 2, comp: "Disolvente",        cant: 0.0119, und: "Galón" },
        { prod: "COMP1.1 - Pieza Aparada 1",     nivel: 2, comp: "Jebe Líquido",      cant: 0.0156, und: "Galón" },
        { prod: "COMP1.1 - Pieza Aparada 1",     nivel: 2, comp: "Pegamentos",        cant: 0.0125, und: "Galón" },

        // ── COMP 1.2: Plantilla A ────────────────────────────────────
        { prod: "COMP1.2 - Plantilla A",         nivel: 2, comp: "Badana",            cant: 0.4,    und: "Pie2" },
        { prod: "COMP1.2 - Plantilla A",         nivel: 2, comp: "Hilos",             cant: 0.0033, und: "Metro" },
        { prod: "COMP1.2 - Plantilla A",         nivel: 2, comp: "Pegamentos",        cant: 0.0031, und: "Galón" },
        { prod: "COMP1.2 - Plantilla A",         nivel: 2, comp: "Látex",             cant: 0.0083, und: "Metro" },
        { prod: "COMP1.2 - Plantilla A",         nivel: 2, comp: "Etiqueta",          cant: 2,      und: "Unidad" },

        // ── COMP 1.3: Falsa (SKU1) ───────────────────────────────────
        { prod: "COMP1.3 - Falsa SKU1",          nivel: 2, comp: "Contrafuertes",     cant: 0.0083, und: "Plancha" },
        { prod: "COMP1.3 - Falsa SKU1",          nivel: 2, comp: "Látex",             cant: 0.0083, und: "Metro" },

        // ── COMP 2.1: Pieza Aparada 5 ────────────────────────────────
        { prod: "COMP2.1 - Pieza Aparada 5",     nivel: 2, comp: "Hilos",             cant: 0.0167, und: "Cono" },
        { prod: "COMP2.1 - Pieza Aparada 5",     nivel: 2, comp: "Cuero",             cant: 3.3333, und: "Pie2" },
        { prod: "COMP2.1 - Pieza Aparada 5",     nivel: 2, comp: "Badana",            cant: 3.75,   und: "Pie2" },
        { prod: "COMP2.1 - Pieza Aparada 5",     nivel: 2, comp: "Lona",              cant: 0.0167, und: "Metro" },
        { prod: "COMP2.1 - Pieza Aparada 5",     nivel: 2, comp: "Contrafuertes",     cant: 0.0194, und: "Plancha" },
        { prod: "COMP2.1 - Pieza Aparada 5",     nivel: 2, comp: "Cintillo",          cant: 0.0167, und: "Cono" },
        { prod: "COMP2.1 - Pieza Aparada 5",     nivel: 2, comp: "Disolvente",        cant: 0.0119, und: "Galón" },
        { prod: "COMP2.1 - Pieza Aparada 5",     nivel: 2, comp: "Jebe Líquido",      cant: 0.0156, und: "Galón" },
        { prod: "COMP2.1 - Pieza Aparada 5",     nivel: 2, comp: "Pegamentos",        cant: 0.0042, und: "Galón" },

        // ── COMP 2.2: Plantilla B ────────────────────────────────────
        { prod: "COMP2.2 - Plantilla B",         nivel: 2, comp: "Badana",            cant: 0.5,    und: "Pie2" },
        { prod: "COMP2.2 - Plantilla B",         nivel: 2, comp: "Pegamentos",        cant: 0.001,  und: "Galón" },
        { prod: "COMP2.2 - Plantilla B",         nivel: 2, comp: "Látex",             cant: 0.008,  und: "Metro" },
        { prod: "COMP2.2 - Plantilla B",         nivel: 2, comp: "Etiqueta",          cant: 2,      und: "Unidad" },

        // ── COMP 2.3: Falsa (SKU2) ───────────────────────────────────
        { prod: "COMP2.3 - Falsa SKU2",          nivel: 2, comp: "Contrafuertes",     cant: 0.0083, und: "Plancha" },
        { prod: "COMP2.3 - Falsa SKU2",          nivel: 2, comp: "Látex",             cant: 0.0083, und: "Metro" },
    ];

    let charts = {};

    // ================= UTILIDAD EXCEL =================
    // Convierte número de columna (0-based) a letra: 0→A, 1→B, 25→Z, 26→AA...
    function colLetra(n) {
        let s = '';
        n += 1;
        while (n > 0) { let r = (n - 1) % 26; s = String.fromCharCode(65 + r) + s; n = Math.floor((n - 1) / 26); }
        return s;
    }
    // Referencia de celda: col (0-based), row (0-based) → "A1"
    function ref(col, row) { return colLetra(col) + (row + 1); }

    // Escribe una hoja usando API de celdas (permite fórmulas)
    // cells = [{c, r, v, f, t}] donde f=formula, v=valor, t=tipo('n','s','f')
    function construirHoja(cells, nCols, nRows) {
        const ws = {};
        cells.forEach(({ c, r, v, f, t }) => {
            const addr = ref(c, r);
            if (f) {
                ws[addr] = { t: 'n', f: f, v: v };          // celda con fórmula
            } else {
                ws[addr] = { t: t || (typeof v === 'number' ? 'n' : 's'), v: v ?? '' };
            }
        });
        ws['!ref'] = `A1:${ref(nCols - 1, nRows - 1)}`;
        return ws;
    }

    function descargarExcel(nombreArchivo, nombreHoja, ws) {
        const wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, nombreHoja);
        XLSX.writeFile(wb, nombreArchivo + '.xlsx');
    }

    // Helper para celda texto
    function ct(c, r, v) { return { c, r, v: String(v), t: 's' }; }
    // Helper para celda número
    function cn(c, r, v) { return { c, r, v: Number(v), t: 'n' }; }
    // Helper para celda con fórmula
    function cf(c, r, formula, valorPreview) { return { c, r, f: formula, v: valorPreview ?? 0 }; }

    // =====================================================
    // GRÁFICO NATIVO EXCEL — OOXML manual con JSZip
    // =====================================================
    async function descargarExcelConGrafico(nombreArchivo, nombreHoja, ws, chartCfg) {
        const JSZip = window.JSZip;
        if (!JSZip) { alert('JSZip no cargado, reintenta en 2 s.'); return; }
        const wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, nombreHoja);
        const buf = XLSX.write(wb, { bookType: 'xlsx', type: 'array' });
        const zip = await JSZip.loadAsync(buf);
        const sheet = nombreHoja.replace(/['"]/g, '');

        // --- chart1.xml ---
        zip.file('xl/charts/chart1.xml', buildChartXml(chartCfg, sheet));
        zip.file('xl/charts/_rels/chart1.xml.rels',
            '<?xml version="1.0" encoding="UTF-8" standalone="yes"?>' +
            '<Relationships xmlns="http://schemas.openxmlformats.org/package/2006/relationships"></Relationships>');

        // --- drawing1.xml ---
        zip.file('xl/drawings/drawing1.xml',
`<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<xdr:wsDr xmlns:xdr="http://schemas.openxmlformats.org/drawingml/2006/spreadsheetDrawing"
  xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main"
  xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships">
  <xdr:twoCellAnchor editAs="oneCell">
    <xdr:from><xdr:col>${chartCfg.fromCol}</xdr:col><xdr:colOff>0</xdr:colOff><xdr:row>${chartCfg.fromRow}</xdr:row><xdr:rowOff>0</xdr:rowOff></xdr:from>
    <xdr:to><xdr:col>${chartCfg.toCol}</xdr:col><xdr:colOff>0</xdr:colOff><xdr:row>${chartCfg.toRow}</xdr:row><xdr:rowOff>0</xdr:rowOff></xdr:to>
    <xdr:graphicFrame macro=""><xdr:nvGraphicFramePr>
      <xdr:cNvPr id="2" name="Grafico 1"/><xdr:cNvGraphicFramePr/>
    </xdr:nvGraphicFramePr>
    <xdr:xfrm><a:off x="0" y="0"/><a:ext cx="0" cy="0"/></xdr:xfrm>
    <a:graphic><a:graphicData uri="http://schemas.openxmlformats.org/drawingml/2006/chart">
      <c:chart xmlns:c="http://schemas.openxmlformats.org/drawingml/2006/chart" r:id="rId1"/>
    </a:graphicData></a:graphic>
    </xdr:graphicFrame><xdr:clientData/>
  </xdr:twoCellAnchor>
</xdr:wsDr>`
            .replace('${chartCfg.fromCol}', chartCfg.fromCol)
            .replace('${chartCfg.fromRow}', chartCfg.fromRow)
            .replace('${chartCfg.toCol}',   chartCfg.toCol)
            .replace('${chartCfg.toRow}',   chartCfg.toRow)
        );
        zip.file('xl/drawings/_rels/drawing1.xml.rels',
            '<?xml version="1.0" encoding="UTF-8" standalone="yes"?>' +
            '<Relationships xmlns="http://schemas.openxmlformats.org/package/2006/relationships">' +
            '<Relationship Id="rId1" ' +
            'Type="http://schemas.openxmlformats.org/officeDocument/2006/relationships/chart" ' +
            'Target="../charts/chart1.xml"/></Relationships>');

        // --- Parchear sheet1.xml ---
        const shKey = 'xl/worksheets/sheet1.xml';
        let shXml = await zip.file(shKey).async('string');
        if (!shXml.includes('<drawing')) {
            shXml = shXml.replace('</worksheet>', '<drawing r:id="rId_dw1"/></worksheet>');
            zip.file(shKey, shXml);
        }

        // --- Parchear _rels/sheet1.xml.rels ---
        const rkKey = 'xl/worksheets/_rels/sheet1.xml.rels';
        const rkFile = zip.file(rkKey);
        const drawRel =
            '<Relationship Id="rId_dw1" ' +
            'Type="http://schemas.openxmlformats.org/officeDocument/2006/relationships/drawing" ' +
            'Target="../drawings/drawing1.xml"/>';
        let rkXml = rkFile ? await rkFile.async('string') : '';
        if (rkXml && !rkXml.includes('drawing1.xml')) {
            rkXml = rkXml.replace('</Relationships>', drawRel + '</Relationships>');
        } else if (!rkXml) {
            rkXml = '<?xml version="1.0" encoding="UTF-8" standalone="yes"?>' +
                '<Relationships xmlns="http://schemas.openxmlformats.org/package/2006/relationships">' +
                drawRel + '</Relationships>';
        }
        zip.file(rkKey, rkXml);

        // --- [Content_Types].xml ---
        let ct2 = await zip.file('[Content_Types].xml').async('string');
        if (!ct2.includes('drawing1.xml')) {
            ct2 = ct2.replace('</Types>',
                '<Override PartName="/xl/drawings/drawing1.xml" ContentType="application/vnd.openxmlformats-officedocument.drawing+xml"/>' +
                '<Override PartName="/xl/charts/chart1.xml" ContentType="application/vnd.openxmlformats-officedocument.drawingml.chart+xml"/>' +
                '</Types>');
            zip.file('[Content_Types].xml', ct2);
        }

        // --- Descargar ---
        const blob = await zip.generateAsync({ type: 'blob',
            mimeType: 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet' });
        const url = URL.createObjectURL(blob);
        const a = document.createElement('a');
        a.href = url; a.download = nombreArchivo + '.xlsx'; a.click();
        setTimeout(() => URL.revokeObjectURL(url), 3000);
    }

    // Construye chartXml OOXML para gráfico de líneas o dispersión
    function buildChartXml(cfg, sheet) {
        const rng = (col, r1, r2) => "'" + sheet + "'!$" + col + "$" + r1 + ":$" + col + "$" + r2;

        const spLn  = (hex) => '<c:spPr><a:ln w="25400"><a:solidFill><a:srgbClr val="' + hex + '"/></a:solidFill></a:ln></c:spPr>';
        const spMk  = (hex) => '<c:spPr><a:solidFill><a:srgbClr val="' + hex + '"/></a:solidFill></c:spPr>';
        const mkLbl = (lbl) => '<c:tx><c:strRef><c:f>"' + lbl + '"</c:f>' +
            '<c:strCache><c:ptCount val="1"/><c:pt idx="0"><c:v>' + lbl + '</c:v></c:pt></c:strCache></c:strRef></c:tx>';
        const mkMkr = (hex, sym) => '<c:marker><c:symbol val="' + sym + '"/><c:size val="5"/>' +
            '<c:spPr><a:solidFill><a:srgbClr val="' + hex + '"/></a:solidFill></c:spPr></c:marker>';

        const serieLn = (idx, s) =>
            '<c:ser><c:idx val="' + idx + '"/><c:order val="' + idx + '"/>' +
            mkLbl(s.label) + spLn(s.color) + mkMkr(s.color, 'circle') +
            '<c:cat><c:strRef><c:f>' + rng(s.catCol, s.r1, s.r2) + '</c:f></c:strRef></c:cat>' +
            '<c:val><c:numRef><c:f>' + rng(s.valCol, s.r1, s.r2) + '</c:f></c:numRef></c:val>' +
            '<c:smooth val="0"/></c:ser>';

        const serieXY = (idx, s) =>
            '<c:ser><c:idx val="' + idx + '"/><c:order val="' + idx + '"/>' +
            mkLbl(s.label) + (s.isLine ? spLn(s.color) : spMk(s.color)) +
            mkMkr(s.color, s.isLine ? 'none' : 'circle') +
            '<c:xVal><c:numRef><c:f>' + rng(s.xCol, s.r1, s.r2) + '</c:f></c:numRef></c:xVal>' +
            '<c:yVal><c:numRef><c:f>' + rng(s.yCol, s.r1, s.r2) + '</c:f></c:numRef></c:yVal>' +
            '<c:smooth val="0"/></c:ser>';

        const axis = (id1, id2, ejeX, ejeY, tipo) => {
            const catTag = tipo === 'linea' ? 'c:catAx' : 'c:valAx';
            return '<' + catTag + '><c:axId val="' + id1 + '"/>' +
                '<c:scaling><c:orientation val="minMax"/></c:scaling>' +
                '<c:delete val="0"/><c:axPos val="b"/>' +
                '<c:title><c:tx><c:rich><a:bodyPr/><a:lstStyle/>' +
                '<a:p><a:r><a:t>' + ejeX + '</a:t></a:r></a:p>' +
                '</c:rich></c:tx><c:overlay val="0"/></c:title>' +
                '<c:numFmt formatCode="General" sourceLinked="1"/>' +
                '<c:crossAx val="' + id2 + '"/></' + catTag + '>' +
                '<c:valAx><c:axId val="' + id2 + '"/>' +
                '<c:scaling><c:orientation val="minMax"/></c:scaling>' +
                '<c:delete val="0"/><c:axPos val="l"/>' +
                '<c:title><c:tx><c:rich><a:bodyPr/><a:lstStyle/>' +
                '<a:p><a:r><a:t>' + ejeY + '</a:t></a:r></a:p>' +
                '</c:rich></c:tx><c:overlay val="0"/></c:title>' +
                '<c:numFmt formatCode="General" sourceLinked="1"/>' +
                '<c:crossAx val="' + id1 + '"/></c:valAx>';
        };

        let plotArea = '';
        if (cfg.tipo === 'linea') {
            const series = cfg.series.map((s,i) => serieLn(i, s)).join('');
            plotArea = '<c:lineChart><c:barDir val="bar"/><c:grouping val="standard"/>' +
                '<c:varyColors val="0"/>' + series +
                '<c:smooth val="0"/><c:axId val="100"/><c:axId val="101"/></c:lineChart>' +
                axis(100, 101, cfg.ejeX||'Período', cfg.ejeY||'Valor', 'linea');
        } else {
            const series = cfg.series.map((s,i) => serieXY(i, s)).join('');
            plotArea = '<c:scatterChart><c:scatterStyle val="lineMarker"/>' +
                '<c:varyColors val="0"/>' + series +
                '<c:axId val="100"/><c:axId val="101"/></c:scatterChart>' +
                axis(100, 101, cfg.ejeX||'X', cfg.ejeY||'Y', 'scatter');
        }

        return '<?xml version="1.0" encoding="UTF-8" standalone="yes"?>' +
            '<c:chartSpace xmlns:c="http://schemas.openxmlformats.org/drawingml/2006/chart"' +
            ' xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main"' +
            ' xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships">' +
            '<c:chart>' +
            '<c:title><c:tx><c:rich><a:bodyPr/><a:lstStyle/>' +
            '<a:p><a:pPr><a:defRPr b="1" sz="1100"/></a:pPr>' +
            '<a:r><a:t>' + cfg.titulo + '</a:t></a:r></a:p>' +
            '</c:rich></c:tx><c:overlay val="0"/></c:title>' +
            '<c:autoTitleDeleted val="0"/>' +
            '<c:plotArea>' + plotArea + '</c:plotArea>' +
            '<c:legend><c:legendPos val="b"/></c:legend>' +
            '<c:plotVisOnly val="1"/></c:chart>' +
            '<c:spPr><a:solidFill><a:srgbClr val="FFFFFF"/></a:solidFill>' +
            '<a:ln><a:solidFill><a:srgbClr val="CCCCCC"/></a:solidFill></a:ln></c:spPr>' +
            '</c:chartSpace>';
    }

    // ================= INTERPRETACIÓN IA =================
    function interpretacionIA(tipo, datos) {
        if (tipo === 'pm') {
            let dam = datos.dam;
            if (dam < 20) return { texto: "✅ Excelente precisión! El modelo se ajusta muy bien a los datos históricos.", clase: "success", recomendacion: "Puedes confiar en este pronóstico para la planificación." };
            if (dam < 50) return { texto: "📈 Precisión moderada. El modelo captura la tendencia general.", clase: "", recomendacion: "Considera combinar con otros métodos para mejorar." };
            return { texto: "⚠️ Baja precisión. Los errores son significativos.", clase: "warning", recomendacion: "Prueba con otro valor de k o utiliza suavizado exponencial." };
        }
        if (tipo === 'reg') {
            let r2 = datos.r2;
            if (r2 > 0.7) return { texto: "✅ Fuerte relación lineal! El modelo explica bien la variabilidad.", clase: "success", recomendacion: "Útil para pronósticos a mediano plazo." };
            if (r2 > 0.4) return { texto: "📈 Relación lineal moderada. El modelo tiene poder predictivo limitado.", clase: "", recomendacion: "Considera agregar más variables o usar otro método." };
            return { texto: "⚠️ Relación lineal débil. La demanda no sigue una tendencia clara.", clase: "warning", recomendacion: "Usa promedios móviles en lugar de regresión." };
        }
        if (tipo === 'pap') {
            let costo = datos.costo;
            if (costo < 180000) return { texto: "✅ Excelente! Costos optimizados. La estrategia elegida es eficiente.", clase: "success", recomendacion: "Mantener esta política de producción." };
            if (costo < 250000) return { texto: "📈 Costos aceptables. Se pueden buscar mejoras.", clase: "", recomendacion: "Revisar niveles de inventario para reducir costos de mantener." };
            return { texto: "⚠️ Costos elevados. La estrategia actual no es óptima.", clase: "danger", recomendacion: "Considerar cambiar a estrategia de persecución o revisar costos unitarios." };
        }
        if (tipo === 'mrp') {
            if (datos.stockFinal < 0) return { texto: "⚠️ ALERTA: Stock negativo detectado! Necesitas generar una orden de compra.", clase: "danger", recomendacion: `Generar orden por ${Math.abs(datos.stockFinal)} unidades con lead time de ${datos.lt} semanas.` };
            if (datos.stockFinal < 50) return { texto: "📉 Stock bajo. Riesgo de desabastecimiento en próximas semanas.", clase: "warning", recomendacion: "Revisar si es necesario pedir antes del próximo ciclo." };
            return { texto: "✅ Stock suficiente. El inventario cubre las necesidades planificadas.", clase: "success", recomendacion: "Monitorear consumo para evitar excesos." };
        }
        return { texto: "Análisis completado.", clase: "", recomendacion: "" };
    }

    // ================= FUNCIONES =================
    function mostrarTablaInventarios() {
        let html = '';
        inventariosData.forEach((item, idx) => {
            html += `<tr>
                <td><input type="text" id="mat_${idx}" value="${item.material.replace(/"/g,'&quot;')}" style="width:180px" placeholder="Nombre del material"></td>
                <td><input type="text" id="und_${idx}" value="${item.und}" style="width:55px" placeholder="Und"></td>
                <td><input type="number" id="stock_${idx}" value="${item.stock}" style="width:75px" placeholder="0"></td>
                <td><input type="text" id="lote_${idx}" value="${item.lote}" style="width:75px" placeholder="LFL o número"></td>
                <td><input type="number" id="lt_${idx}" value="${item.lt}" style="width:55px" placeholder="0"></td>
                <td><button onclick="eliminarFilaInventario(${idx})" style="background:#883c2c;padding:0.2rem 0.5rem;margin:0;border-radius:0.4rem;font-size:0.72rem">
                    <i class="fas fa-trash"></i>
                </button></td>
            </tr>`;
        });
        document.querySelector("#tblInventarios tbody").innerHTML = html;
    }

    function guardarInventarios() {
        sincronizarInventarios();
        // También actualizar nombre y unidad que sincronizarInventarios no lee
        for(let i=0; i<inventariosData.length; i++) {
            const matEl = document.getElementById(`mat_${i}`);
            const undEl = document.getElementById(`und_${i}`);
            if (matEl) inventariosData[i].material = matEl.value.trim();
            if (undEl) inventariosData[i].und = undEl.value.trim();
        }
        alert("✅ Inventarios guardados correctamente");
        poblarSelectMRP();
        generarOrdenesAprovisionamiento();
    }

    function agregarFilaInventario() {
        inventariosData.push({ material: '', und: 'Pza', stock: 0, lote: 'LFL', lt: 0 });
        mostrarTablaInventarios();
        // Scroll al final de la tabla
        const tabla = document.getElementById('tblInventarios');
        if (tabla) tabla.scrollIntoView({ behavior: 'smooth', block: 'end' });
    }

    function eliminarFilaInventario(idx) {
        if (!confirm(`¿Eliminar "${inventariosData[idx].material || 'esta fila'}"?`)) return;
        inventariosData.splice(idx, 1);
        mostrarTablaInventarios();
    }

    let editandoBOM = false;

    // productoEditando = nombre del producto en edición (null = ninguno)
    let productoEditando = null;

    function mostrarBOM() {
        // Agrupar por producto manteniendo orden de aparición
        const grupos = {};
        const orden  = [];
        bomData.forEach((item, idx) => {
            if (!grupos[item.prod]) { grupos[item.prod] = []; orden.push(item.prod); }
            grupos[item.prod].push({ ...item, _idx: idx });
        });

        const nivelColor = ['#00f2fe','#4facfe','#4ade80','#facc15','#c084fc'];
        const nivelPad   = [0, 14, 28, 42, 56];
        const th = t => `<th style="background:#10323e;color:#a5f3fc;padding:4px 8px;font-size:0.75rem">${t}</th>`;

        let html3 = '';
        orden.forEach(prod => {
            const items   = grupos[prod];
            const editar  = productoEditando === prod;
            const safeId  = prod.replace(/[^a-zA-Z0-9]/g, '_');

            html3 += `
            <details open id="det_${safeId}" style="margin-bottom:0.6rem;border:1px solid ${editar?'#facc15':'#2a4b5c'};border-radius:0.6rem;overflow:hidden">
                <summary style="cursor:pointer;background:${editar?'#1f2a0f':'#0f2535'};padding:0.5rem 0.8rem;
                    display:flex;align-items:center;gap:0.5rem;list-style:none;user-select:none">
                    <span style="font-size:1rem">📦</span>
                    ${editar
                        ? `<input type="text" id="edit_prod_nombre_${safeId}" value="${prod.replace(/"/g,'&quot;')}"
                            style="font-size:0.85rem;font-weight:700;color:#facc15;background:rgba(250,204,21,0.1);
                            border:1px solid #facc15;border-radius:0.4rem;padding:2px 8px;width:220px"
                            onclick="event.stopPropagation()" placeholder="Nombre del producto">`
                        : `<strong style="color:#eef2ff;font-size:0.85rem">${prod}</strong>`
                    }
                    <span style="font-size:0.7rem;color:#8bb3cc">${items.length} componente(s)</span>
                    <div style="margin-left:auto;display:flex;gap:0.4rem" onclick="event.stopPropagation()">
                        ${editar
                            ? `<button onclick="guardarProductoBOM('${prod.replace(/'/g,"\'")}')"
                                style="background:#1a5c2a;padding:0.2rem 0.7rem;margin:0;border-radius:0.4rem;font-size:0.72rem">
                                <i class="fas fa-save"></i> Guardar</button>
                               <button onclick="cancelarEditBOM()"
                                style="background:#883c2c;padding:0.2rem 0.7rem;margin:0;border-radius:0.4rem;font-size:0.72rem">
                                <i class="fas fa-times"></i> Cancelar</button>`
                            : `<button onclick="editarProductoBOM('${prod.replace(/'/g,"\'")}')"
                                style="background:#1f6d7a;padding:0.2rem 0.7rem;margin:0;border-radius:0.4rem;font-size:0.72rem">
                                <i class="fas fa-edit"></i> Editar</button>
                               <button onclick="eliminarProductoBOM('${prod.replace(/'/g,"\'")}')"
                                style="background:#883c2c;padding:0.2rem 0.7rem;margin:0;border-radius:0.4rem;font-size:0.72rem">
                                <i class="fas fa-trash"></i></button>`
                        }
                    </div>
                    <span style="font-size:0.7rem;color:#5f8ca3">▼</span>
                </summary>

                <div style="overflow-x:auto;padding:${editar?'0.5rem':'0'}">
                ${editar ? `
                <!-- Modo edición de este producto -->
                <table style="width:100%;border-collapse:collapse;font-size:0.78rem">
                <thead><tr>${th('Nivel')}${th('Componente')}${th('Cantidad')}${th('Unidad')}${th('Acción')}</tr></thead>
                <tbody id="tbody_edit_${safeId}">
                ${items.map((item,i) => `
                    <tr>
                        <td style="padding:4px 6px"><input type="number" id="edit_nivel_${item._idx}" value="${item.nivel}" style="width:50px" min="0" max="5"></td>
                        <td style="padding:4px 6px"><input type="text"   id="edit_comp_${item._idx}"  value="${item.comp.replace(/"/g,'&quot;')}"  style="width:180px"></td>
                        <td style="padding:4px 6px">
                        <input type="text" id="edit_cant_${item._idx}" value="${item.cant}"
                            style="width:80px" placeholder="Ej: 0.0167"
                            title="Cantidad — acepta decimales como 0.0167">
                    </td>
                    <td style="padding:4px 6px">
                        <input type="text" id="edit_und_${item._idx}" value="${item.und}"
                            style="width:70px" placeholder="Und"
                            list="undList">
                    </td>
                        <td style="padding:4px 6px">
                            <button onclick="eliminarFilaBOM(${item._idx})"
                                style="background:#883c2c;padding:0.15rem 0.5rem;margin:0;border-radius:0.4rem;font-size:0.7rem">
                                <i class="fas fa-trash"></i></button>
                        </td>
                    </tr>`).join('')}
                <!-- Fila nueva -->
                <tr style="background:rgba(0,242,254,0.05)">
                    <td style="padding:4px 6px"><select id="new_nivel_${safeId}" style="width:60px">
                        <option value="0">0</option><option value="1" selected>1</option>
                        <option value="2">2</option><option value="3">3</option><option value="4">4</option>
                    </select></td>
                    <td style="padding:4px 6px"><input type="text"   id="new_comp_${safeId}"  placeholder="Nuevo componente" style="width:180px"></td>
                    <td style="padding:4px 6px"><input type="number" id="new_cant_${safeId}"  placeholder="1" style="width:70px" step="any" min="0"></td>
                    <td style="padding:4px 6px"><input type="text"   id="new_und_${safeId}"   placeholder="Und" style="width:65px"></td>
                    <td style="padding:4px 6px">
                        <button onclick="agregarComponenteBOM('${prod.replace(/'/g,"\'")}')"
                            style="background:#1a5c2a;padding:0.15rem 0.6rem;margin:0;border-radius:0.4rem;font-size:0.7rem">
                            <i class="fas fa-plus"></i> Agregar</button>
                    </td>
                </tr>
                </tbody></table>
                ` : `
                <!-- Modo lectura de este producto -->
                <table style="width:100%;border-collapse:collapse;font-size:0.78rem">
                <thead><tr>${th('Nivel')}${th('Componente')}${th('Cantidad')}${th('Unidad')}</tr></thead>
                <tbody>
                ${items.map(item => `
                    <tr style="border-bottom:1px solid #1a3040">
                        <td style="padding:5px 8px">
                            <span style="background:${nivelColor[item.nivel]||'#555'};color:#0a0e12;
                                padding:1px 7px;border-radius:1rem;font-size:0.68rem;font-weight:700;
                                margin-left:${nivelPad[item.nivel]||0}px">N${item.nivel}</span>
                        </td>
                        <td style="padding:5px 8px;padding-left:${8+(nivelPad[item.nivel]||0)}px">${item.comp}</td>
                        <td style="padding:5px 8px;text-align:right;font-weight:600;color:#a5f3fc">${item.cant}</td>
                        <td style="padding:5px 8px;color:#8bb3cc">${item.und}</td>
                    </tr>`).join('')}
                </tbody></table>`}
                </div>
            </details>`;
        });

        // Botón agregar nuevo producto al final
        html3 += `
        <div style="margin-top:0.5rem;padding:0.6rem;border:1px dashed #2a4b5c;border-radius:0.6rem;display:flex;gap:0.5rem;align-items:center;flex-wrap:wrap">
            <span style="font-size:0.78rem;color:#8bb3cc">Nuevo producto:</span>
            <input type="text" id="nuevo_prod_bom" placeholder="Nombre del producto" style="width:200px">
            <button onclick="agregarNuevoProductoBOM()"
                style="background:#1a5c2a;padding:0.3rem 0.8rem;margin:0;border-radius:0.4rem;font-size:0.78rem">
                <i class="fas fa-plus"></i> Agregar producto</button>
        </div>`;

        if (!orden.length) html3 = `<p style="color:#8bb3cc;font-size:0.85rem">No hay componentes. Agrega un producto nuevo abajo.</p>` + html3;

        document.getElementById('tablaBOM').innerHTML = html3;
        // Mantener tblBOM oculto (ya no se usa directamente)
        if (!document.getElementById('tblBOM')) {
            document.getElementById('tablaBOM').insertAdjacentHTML('beforeend','<table id="tblBOM" style="display:none"></table>');
        }

        // Estado del botón Editar global (lo ocultamos — ahora es por producto)
        const btnEdit = document.getElementById('btnEditarBOM');
        const btnSave = document.getElementById('btnGuardarBOM');
        if (btnEdit) btnEdit.style.display = 'none';
        if (btnSave) btnSave.style.display = 'none';
        document.getElementById('bomEstado').innerText = productoEditando ? `✏️ Editando: ${productoEditando}` : 'Modo Lectura';
        document.getElementById('bomEstado').style.color = productoEditando ? '#facc15' : '#8bb3cc';
    }

    function editarProductoBOM(prod) {
        productoEditando = prod;
        mostrarBOM();
        // Scroll al producto
        const safeId = prod.replace(/[^a-zA-Z0-9]/g,'_');
        const det = document.getElementById(`det_${safeId}`);
        if (det) { det.open = true; det.scrollIntoView({ behavior:'smooth', block:'nearest' }); }
    }

    function cancelarEditBOM() {
        productoEditando = null;
        mostrarBOM();
    }

    function guardarProductoBOM(prod) {
        const safeId    = prod.replace(/[^a-zA-Z0-9]/g,'_');
        // Leer nuevo nombre del producto
        const nombreEl  = document.getElementById(`edit_prod_nombre_${safeId}`);
        const nuevoNombre = nombreEl ? nombreEl.value.trim() : prod;

        if (!nuevoNombre) { alert('⚠️ El nombre del producto no puede estar vacío'); return; }

        // Si cambió el nombre, verificar que no exista otro igual
        if (nuevoNombre !== prod && bomData.some(b => b.prod === nuevoNombre)) {
            alert(`⚠️ Ya existe un producto llamado "${nuevoNombre}"`); return;
        }

        // Actualizar filas de este producto en bomData
        const items = bomData.map((item, idx) => ({ ...item, _idx: idx })).filter(i => i.prod === prod);
        items.forEach(item => {
            const nivelEl = document.getElementById(`edit_nivel_${item._idx}`);
            const compEl  = document.getElementById(`edit_comp_${item._idx}`);
            const cantEl  = document.getElementById(`edit_cant_${item._idx}`);
            const undEl   = document.getElementById(`edit_und_${item._idx}`);
            if (nivelEl) bomData[item._idx].nivel = parseInt(nivelEl.value) ?? 0;
            if (compEl)  bomData[item._idx].comp  = compEl.value.trim();
            if (cantEl)  { const v = parseFloat(cantEl.value.replace(',','.')); bomData[item._idx].cant = isNaN(v) ? 1 : v; }
            if (undEl)   bomData[item._idx].und   = undEl.value.trim();
            // Renombrar el producto en todas sus filas
            bomData[item._idx].prod = nuevoNombre;
        });

        productoEditando = null;
        mostrarBOM();
        cargarSKUsdesdeBOM();
        generarOrdenesAprovisionamiento();
    }

    function eliminarProductoBOM(prod) {
        if (!confirm(`¿Eliminar el producto "${prod}" y todos sus componentes del BOM?`)) return;
        const antes = bomData.length;
        for (let i = bomData.length - 1; i >= 0; i--) {
            if (bomData[i].prod === prod) bomData.splice(i, 1);
        }
        productoEditando = null;
        mostrarBOM();
        generarOrdenesAprovisionamiento();
    }

    function agregarComponenteBOM(prod) {
        const safeId  = prod.replace(/[^a-zA-Z0-9]/g,'_');
        const nivelEl = document.getElementById(`new_nivel_${safeId}`);
        const compEl  = document.getElementById(`new_comp_${safeId}`);
        const cantEl  = document.getElementById(`new_cant_${safeId}`);
        const undEl   = document.getElementById(`new_und_${safeId}`);
        const comp = compEl?.value.trim();
        const cant = parseFloat(cantEl?.value);
        if (!comp || isNaN(cant)) { alert('⚠️ Completa Componente y Cantidad'); return; }
        bomData.push({
            prod,
            nivel: parseInt(nivelEl?.value) || 1,
            comp, cant,
            und: undEl?.value.trim() || ''
        });
        // Mantener en modo edición para seguir agregando
        mostrarBOM();
        editarProductoBOM(prod);
    }

    function agregarNuevoProductoBOM() {
        const el = document.getElementById('nuevo_prod_bom');
        const prod = el?.value.trim();
        if (!prod) { alert('⚠️ Ingresa el nombre del producto'); return; }
        if (bomData.some(b => b.prod === prod)) { alert(`⚠️ "${prod}" ya existe en el BOM`); return; }
        // Agregar fila nivel 0 automáticamente
        bomData.push({ prod, nivel: 0, comp: 'Producto Final', cant: 1, und: 'Doc' });
        mostrarBOM();
        editarProductoBOM(prod);
    }


    function guardarBOM() {
        // Lee todos los inputs de las filas existentes y actualiza bomData
        const nuevaBOM = [];
        bomData.forEach((_, idx) => {
            const prod  = document.getElementById(`bom_prod_${idx}`)?.value.trim();
            const nivel = parseInt(document.getElementById(`bom_nivel_${idx}`)?.value);
            const comp  = document.getElementById(`bom_comp_${idx}`)?.value.trim();
            const cant  = parseFloat(document.getElementById(`bom_cant_${idx}`)?.value);
            const und   = document.getElementById(`bom_und_${idx}`)?.value.trim();
            if (prod && comp) nuevaBOM.push({ prod, nivel: isNaN(nivel) ? 0 : nivel, comp, cant: isNaN(cant) ? 1 : cant, und: und || '' });
        });
        bomData = nuevaBOM;
        editandoBOM = false;
        mostrarBOM();
        cargarSKUsdesdeBOM(); // actualizar labels PMP con nuevos nombres del BOM
        generarOrdenesAprovisionamiento();
        alert('✅ BOM guardado correctamente');
    }

    function eliminarFilaBOM(idx) {
        if (confirm(`¿Eliminar "${bomData[idx].comp}" del BOM?`)) {
            bomData.splice(idx, 1);
            mostrarBOM();
            generarOrdenesAprovisionamiento();
        }
    }

    function agregarFilaBOM() {
        const prod  = document.getElementById('nuevo_prod')?.value.trim();
        const nivel = parseInt(document.getElementById('nuevo_nivel')?.value);
        const comp  = document.getElementById('nuevo_comp')?.value.trim();
        const cant  = parseFloat(document.getElementById('nuevo_cant')?.value);
        const und   = document.getElementById('nuevo_und')?.value.trim();
        if (!prod || !comp || isNaN(cant)) {
            alert('⚠️ Completa al menos: Producto, Componente y Cantidad');
            return;
        }
        bomData.push({ prod, nivel: isNaN(nivel) ? 0 : nivel, comp, cant, und: und || '' });
        mostrarBOM();
        generarOrdenesAprovisionamiento();
    }


    function calcularPM() {
        const datosStrPM = document.getElementById('datosPM').value.trim();
        if (!datosStrPM) { alert('⚠️ Ingresa los datos históricos separados por comas'); return; }
        let datos = datosStrPM.split(',').map(Number);
        if (datos.some(isNaN)) { alert('⚠️ Los datos deben ser números separados por comas'); return; }
        let k = parseInt(document.getElementById('kPM').value);
        if (isNaN(k) || k < 1) { alert("Ingrese un k válido (entero positivo)"); return; }
        if(datos.length < k) { alert("Se requieren más datos que el valor de k"); return; }

        // Pronósticos: desde el período k+1 en adelante
        let pronosticos = []; // pronosticos[i] = pronóstico para datos[k+i]
        for(let i=k; i<datos.length; i++) {
            let suma = 0;
            for(let j=i-k; j<i; j++) suma += datos[j];
            pronosticos.push(suma/k);
        }
        // Pronóstico del siguiente período (período n+1)
        let suma = 0;
        for(let j=datos.length-k; j<datos.length; j++) suma += datos[j];
        let pronosticoSig = suma/k;
        let todosPronosticos = pronosticos.concat([pronosticoSig]);

        // Errores: error[i] = datos[k+i] - pronosticos[i]
        let errores = pronosticos.map((p,i) => datos[k+i] - p);
        let absErr  = errores.map(e => Math.abs(e));
        let DAM  = absErr.reduce((a,b)=>a+b,0) / errores.length;
        let ECM  = errores.map(e=>e*e).reduce((a,b)=>a+b,0) / errores.length;
        // EPAM = promedio de |error_i / demanda_i| (mismo que Excel)
        let PEMA = errores.map((e,i)=>Math.abs(e/datos[k+i])).reduce((a,b)=>a+b,0) / errores.length * 100;

        _datosPM = datos; _pronosticosPM = todosPronosticos; _kPM = k;
        _damPM = DAM; _ecmPM = ECM; _pemaPM = PEMA;

        // Tabla de resultados
        let filas = datos.map((d,i) => {
            if(i < k) return `<tr><td>Mes ${i+1}</td><td>${d}</td><td>—</td><td>—</td><td>—</td><td>—</td></tr>`;
            let p = pronosticos[i-k];
            let e = d - p;
            return `<tr><td>Mes ${i+1}</td><td>${d}</td><td>${p.toFixed(2)}</td><td>${e.toFixed(2)}</td><td>${Math.abs(e).toFixed(2)}</td><td>${(Math.abs(e/d)*100).toFixed(2)}%</td></tr>`;
        }).join('');

        let ia = interpretacionIA('pm', { dam: DAM });
        let html = `<table><thead><tr><th>Período</th><th>Demanda</th><th>Pronóstico PM</th><th>Error</th><th>|Error|</th><th>EPAM</th></tr></thead><tbody>${filas}</tbody></table>
                    <p style="margin-top:0.5rem"><strong>📊 Pronóstico mes ${datos.length+1}:</strong> <strong style="color:#00f2fe">${pronosticoSig.toFixed(2)}</strong> unidades</p>
                    <p><strong>DAM:</strong> ${DAM.toFixed(4)} &nbsp;|&nbsp; <strong>ECM:</strong> ${ECM.toFixed(4)} &nbsp;|&nbsp; <strong>EPAM:</strong> ${PEMA.toFixed(4)}%</p>
                    <div class="ia-insight ${ia.clase}"><i class="fas fa-robot"></i> <strong>🤖 IA:</strong> ${ia.texto} ${ia.recomendacion}</div>`;
        document.getElementById('resultadoPM').innerHTML = html;

        if (charts.pm) charts.pm.destroy();
        let ctx = document.getElementById('chartPM').getContext('2d');
        let etiquetas = datos.map((_,i)=>`M${i+1}`);
        let datosPronostico = Array(k).fill(null).concat(pronosticos.slice(0,-1));
        charts.pm = new Chart(ctx, {
            type: 'line',
            plugins: [{ id:'bgWhite', beforeDraw(c){ const ctx=c.ctx; ctx.save(); ctx.fillStyle='#ffffff'; ctx.fillRect(0,0,c.width,c.height); ctx.restore(); } }],
            data: { labels: etiquetas, datasets: [
                { label: 'Histórico', data: datos, borderColor: '#1a6fa8', backgroundColor: 'rgba(26,111,168,0.1)', tension: 0.3, pointBackgroundColor:'#1a6fa8' },
                { label: `Pronóstico (k=${k})`, data: datosPronostico, borderColor: '#e8a020', borderDash: [5,5], pointBackgroundColor:'#e8a020' }
            ]},
            options: { plugins: { legend: { labels: { color:'#333' } } }, scales: { x: { ticks:{color:'#333'} }, y: { ticks:{color:'#333'} } } }
        });
    }

    function exportarExcelPM() {
        if (!_datosPM.length) { alert("Primero calcula el Promedio Móvil"); return; }
        const k = _kPM;
        const n = _datosPM.length;
        const cells = [];
        let r = 0;

        // Títulos
        cells.push(ct(0, r++, 'Sistema IA de Planificación - Leonardo Carrasco Ocon'));
        cells.push(ct(0, r++, `Promedio Móvil Simple (k=${k})`));
        r++; // fila vacía

        // Encabezados
        ['Período','Demanda Real','Pronóstico PM','Error (D-P)','|Error|','Error²'].forEach((h,c) => cells.push(ct(c, r, h)));
        r++;
        const dataStartRow = r; // fila donde empieza la fila 1 de datos (0-based)

        // Datos y fórmulas fila por fila
        _datosPM.forEach((d, i) => {
            const rr = r + i;
            const colD = 'B'; // Demanda Real en columna B
            const colP = 'C'; // Pronóstico en columna C
            const colE = 'D'; // Error
            const colAE = 'E'; // |Error|
            const colE2 = 'F'; // Error²
            const excelRow = rr + 1; // 1-based para fórmulas

            cells.push(ct(0, rr, `Mes ${i+1}`));
            cells.push(cn(1, rr, d));

            if (i >= k) {
                // Fórmula: promedio de las k celdas anteriores en columna B
                const rangeStart = `B${dataStartRow + i - k + 1}`;
                const rangeEnd   = `B${dataStartRow + i}`;
                cells.push(cf(2, rr, `AVERAGE(${rangeStart}:${rangeEnd})`, Number(_pronosticosPM[i-k].toFixed(4))));
                cells.push(cf(3, rr, `${colD}${excelRow}-${colP}${excelRow}`, Number((_datosPM[i]-_pronosticosPM[i-k]).toFixed(4))));
                cells.push(cf(4, rr, `ABS(${colE}${excelRow})`, Math.abs(_datosPM[i]-_pronosticosPM[i-k])));
                cells.push(cf(5, rr, `${colE}${excelRow}^2`, Math.pow(_datosPM[i]-_pronosticosPM[i-k],2)));
            } else {
                cells.push(ct(2, rr, ''));
                cells.push(ct(3, rr, '')); cells.push(ct(4, rr, '')); cells.push(ct(5, rr, ''));
            }
        });

        const lastDataRow = r + n; // fila siguiente al último dato (0-based)
        r += n;
        r++; // fila vacía

        // Pronóstico próximo período
        const pronRow = r;
        cells.push(ct(0, r, 'Pronóstico próximo período'));
        cells.push(ct(1, r, ''));
        const rangeStart = `B${dataStartRow + n - k + 1}`;
        const rangeEnd   = `B${dataStartRow + n}`;
        cells.push(cf(2, r, `AVERAGE(${rangeStart}:${rangeEnd})`, Number(_pronosticosPM[_pronosticosPM.length-1].toFixed(4))));
        r += 2;

        // Indicadores con fórmulas
        const eStartRow = dataStartRow + k + 1; // primera fila con error (1-based)
        const eEndRow   = dataStartRow + n;     // última fila con error (1-based)

        cells.push(ct(0, r, 'Indicadores')); cells.push(ct(1, r, 'Fórmula Excel')); cells.push(ct(2, r, 'Resultado'));
        r++;
        cells.push(ct(0, r, 'DAM (Desv. Abs. Media)'));
        cells.push(ct(1, r, `=AVERAGE(E${eStartRow}:E${eEndRow})`));
        cells.push(cf(2, r, `AVERAGE(E${eStartRow}:E${eEndRow})`, Number(_damPM.toFixed(4))));
        r++;
        cells.push(ct(0, r, 'ECM (Error Cuad. Medio)'));
        cells.push(ct(1, r, `=AVERAGE(F${eStartRow}:F${eEndRow})`));
        cells.push(cf(2, r, `AVERAGE(F${eStartRow}:F${eEndRow})`, Number(_ecmPM.toFixed(4))));
        r++;
        cells.push(ct(0, r, 'PEMA (% Error Abs.)'));
        cells.push(ct(1, r, `=ABS(B${dataStartRow+n}-C${pronRow+1})/B${dataStartRow+n}*100`));
        cells.push(cf(2, r, `ABS(B${dataStartRow+n}-C${pronRow+1})/B${dataStartRow+n}*100`, Number(_pemaPM.toFixed(4))));
        r++;

        const ws = construirHoja(cells, 6, r);
        ws['!cols'] = [28,16,18,18,14,14].map(w=>({wch:w}));
        // dataStartRow es 0-based; en Excel las filas son 1-based
        const r1pm = dataStartRow + 1;
        const r2pm = dataStartRow + n;
        descargarExcelConGrafico(`Promedio_Movil_k${k}`, 'Promedio Móvil', ws, {
            tipo: 'linea',
            titulo: `Promedio Móvil Simple (k=${k})`,
            ejeX: 'Período', ejeY: 'Unidades',
            fromCol: 7, fromRow: 2, toCol: 16, toRow: 22,
            series: [
                { label: 'Demanda Real',       catCol: 'A', valCol: 'B', r1: r1pm, r2: r2pm, color: '1A6FA8' },
                { label: `Pronóstico k=${k}`,  catCol: 'A', valCol: 'C', r1: r1pm, r2: r2pm, color: 'E8A020' }
            ]
        });
    }

    // --- Suavizado Exponencial ---
    let _datosSE = [], _pronosticosSE = [], _alfaSE = 0.3, _damSE = 0, _pronosticoFinalSE = 0;

    function calcularSE() {
        const datosStrSE = document.getElementById('datosSE').value.trim();
        if (!datosStrSE) { alert('⚠️ Ingresa los datos históricos separados por comas'); return; }
        let datos = datosStrSE.split(',').map(Number);
        if (datos.some(isNaN)) { alert('⚠️ Los datos deben ser números separados por comas'); return; }
        let alfa = parseFloat(document.getElementById('alfaSE').value);
        if (isNaN(alfa) || alfa <= 0 || alfa >= 1) { alert("⚠️ Ingresa un alfa (α) entre 0 y 1 (no inclusive)"); return; }

        // F1 = D1 (primer pronóstico igual a primera demanda, como en el Excel)
        let pronosticos = [datos[0]];
        for(let i=1; i<datos.length; i++) pronosticos.push(alfa*datos[i-1] + (1-alfa)*pronosticos[i-1]);
        // Pronóstico siguiente período
        let pronosticoFinal = alfa*datos[datos.length-1] + (1-alfa)*pronosticos[pronosticos.length-1];

        // Errores: incluye todos los períodos (error mes 1 = 0)
        let errores = datos.map((d,i) => d - pronosticos[i]);
        let absErr  = errores.map(e => Math.abs(e));
        let DAM  = absErr.reduce((a,b)=>a+b,0) / datos.length;
        let ECM  = errores.map(e=>e*e).reduce((a,b)=>a+b,0) / datos.length;
        let PEMA = datos.map((d,i) => Math.abs(errores[i]/d)).reduce((a,b)=>a+b,0) / datos.length * 100;

        _datosSE = datos; _pronosticosSE = pronosticos; _alfaSE = alfa;
        _damSE = DAM; _pronosticoFinalSE = pronosticoFinal;

        let filas = datos.map((d,i) => {
            let p = pronosticos[i]; let e = errores[i];
            return `<tr><td>Mes ${i+1}</td><td>${d}</td><td>${p.toFixed(4)}</td><td>${e.toFixed(4)}</td><td>${Math.abs(e).toFixed(4)}</td><td>${(Math.abs(e/d)*100).toFixed(4)}%</td></tr>`;
        }).join('');

        let html2 = `<table><thead><tr><th>Período</th><th>Demanda</th><th>Pronóstico</th><th>Error</th><th>|Error|</th><th>EPAM</th></tr></thead><tbody>${filas}</tbody></table>
                    <p style="margin-top:0.5rem"><strong>📊 Pronóstico mes ${datos.length+1}:</strong> <strong style="color:#00f2fe">${pronosticoFinal.toFixed(4)}</strong></p>
                    <p><strong>DAM:</strong> ${DAM.toFixed(4)} &nbsp;|&nbsp; <strong>ECM:</strong> ${ECM.toFixed(4)} &nbsp;|&nbsp; <strong>EPAM:</strong> ${PEMA.toFixed(4)}%</p>
                    <div class="ia-insight"><i class="fas fa-robot"></i> α=${alfa} pondera más datos ${alfa>=0.5?'recientes':'históricos'}. ${alfa>=0.5?'Útil para demanda volátil.':'Útil para demanda estable.'}</div>`;
        document.getElementById('resultadoSE').innerHTML = html2;

        if (charts.se) charts.se.destroy();
        let ctx = document.getElementById('chartSE').getContext('2d');
        charts.se = new Chart(ctx, {
            type: 'line',
            plugins: [{ id:'bgWhite', beforeDraw(c){ const ctx=c.ctx; ctx.save(); ctx.fillStyle='#ffffff'; ctx.fillRect(0,0,c.width,c.height); ctx.restore(); } }],
            data: { labels: datos.map((_,i)=>`M${i+1}`), datasets: [
                { label: 'Histórico', data: datos, borderColor: '#1a6fa8', backgroundColor:'rgba(26,111,168,0.1)', pointBackgroundColor:'#1a6fa8' },
                { label: `Suavizado (α=${alfa})`, data: pronosticos, borderColor: '#e8a020', backgroundColor:'rgba(232,160,32,0.1)', pointBackgroundColor:'#e8a020' }
            ]},
            options: { plugins: { legend: { labels: { color:'#333' } } }, scales: { x: { ticks:{color:'#333'} }, y: { ticks:{color:'#333'} } } }
        });
    }

    function exportarExcelSE() {
        if (!_datosSE.length) { alert("Primero calcula el Suavizado Exponencial"); return; }
        const n = _datosSE.length;
        const a = _alfaSE;
        const cells = [];
        let r = 0;

        cells.push(ct(0, r++, 'Sistema IA de Planificación - Leonardo Carrasco Ocon'));
        cells.push(ct(0, r++, `Suavizado Exponencial (α=${a})`));
        r++;
        // Parámetro alfa en celda nombrada para que las fórmulas lo referencien
        cells.push(ct(0, r, 'Alfa (α)')); cells.push(cn(1, r, a));
        const alfaRef = `B${r+1}`; // referencia 1-based
        r++;
        r++;

        ['Período','Demanda Real','Pronóstico Suavizado','Error (D-P)','|Error|'].forEach((h,c) => cells.push(ct(c, r, h)));
        r++;
        const ds = r; // dataStart (0-based)

        _datosSE.forEach((d, i) => {
            const rr = r + i;
            const excelRow = rr + 1;
            cells.push(ct(0, rr, `Mes ${i+1}`));
            cells.push(cn(1, rr, d));

            if (i === 0) {
                // Primer pronóstico = primer dato real
                cells.push(cf(2, rr, `B${excelRow}`, _datosSE[0]));
                cells.push(ct(3, rr, '')); cells.push(ct(4, rr, ''));
            } else {
                const prevPronRow = excelRow - 1;
                const prevDemRow  = excelRow - 1;
                // Ft = α * D(t-1) + (1-α) * F(t-1)
                cells.push(cf(2, rr, `${alfaRef}*B${prevDemRow}+(1-${alfaRef})*C${prevPronRow}`, Number(_pronosticosSE[i].toFixed(4))));
                cells.push(cf(3, rr, `B${excelRow}-C${excelRow}`, Number((_datosSE[i]-_pronosticosSE[i]).toFixed(4))));
                cells.push(cf(4, rr, `ABS(D${excelRow})`, Math.abs(_datosSE[i]-_pronosticosSE[i])));
            }
        });

        r += n;
        // Pronóstico siguiente período
        const lastDemRow  = ds + n;     // 1-based
        const lastPronRow = ds + n;
        cells.push(ct(0, r, 'Pronóstico próximo período'));
        cells.push(ct(1, r, ''));
        cells.push(cf(2, r, `${alfaRef}*B${lastDemRow}+(1-${alfaRef})*C${lastPronRow}`, Number(_pronosticoFinalSE.toFixed(4))));
        r += 2;

        const eStart = ds + 2; // primera fila con error (1-based, i=1)
        const eEnd   = ds + n;
        cells.push(ct(0, r, 'DAM')); cells.push(ct(1, r, `=AVERAGE(E${eStart}:E${eEnd})`));
        cells.push(cf(2, r, `AVERAGE(E${eStart}:E${eEnd})`, Number(_damSE.toFixed(4))));

        const ws = construirHoja(cells, 5, r + 1);
        ws['!cols'] = [28,16,22,18,14].map(w=>({wch:w}));
        const r1se = ds + 1;
        const r2se = ds + n;
        descargarExcelConGrafico(`Suavizado_Exponencial_a${a}`, 'Suavizado Exponencial', ws, {
            tipo: 'linea',
            titulo: `Suavizado Exponencial (α=${a})`,
            ejeX: 'Período', ejeY: 'Unidades',
            fromCol: 6, fromRow: 5, toCol: 15, toRow: 25,
            series: [
                { label: 'Demanda Real',        catCol: 'A', valCol: 'B', r1: r1se, r2: r2se, color: '1A6FA8' },
                { label: `Suavizado α=${a}`,     catCol: 'A', valCol: 'C', r1: r1se, r2: r2se, color: 'E8A020' }
            ]
        });
    }

    // --- Regresión ---
    let _datosReg = [], _aReg = 0, _bReg = 0, _rReg = 0, _r2Reg = 0;

    function calcularReg() {
        const datosStrReg = document.getElementById('datosReg').value.trim();
        if (!datosStrReg) { alert('⚠️ Ingresa los datos históricos separados por comas'); return; }
        let datos = datosStrReg.split(',').map(Number);
        if (datos.some(isNaN) || datos.length < 3) { alert('⚠️ Ingresa al menos 3 períodos numéricos'); return; }
        let n = datos.length;
        let x = Array.from({length: n}, (_,i) => i+1);
        let sumX = x.reduce((a,b)=>a+b,0);
        let sumY = datos.reduce((a,b)=>a+b,0);
        let sumXY = 0, sumX2 = 0;
        for(let i=0; i<n; i++) { sumXY += x[i]*datos[i]; sumX2 += x[i]*x[i]; }
        let b = (n*sumXY - sumX*sumY) / (n*sumX2 - sumX*sumX);
        let a = (sumY - b*sumX)/n;
        let rNumerador = n*sumXY - sumX*sumY;
        let rDenom = Math.sqrt((n*sumX2 - sumX*sumX) * (n*datos.reduce((s,yt)=>s+yt*yt,0) - sumY*sumY));
        let r = rNumerador / rDenom;
        let r2 = r*r;

        _datosReg = datos; _aReg = a; _bReg = b; _rReg = r; _r2Reg = r2;

        let ia = interpretacionIA('reg', { r2: r2 });

        let html = `<p><strong>📐 Ecuación:</strong> y = ${a.toFixed(2)} + ${b.toFixed(4)}x</p>
                    <p><strong>📊 r (Correlación):</strong> ${r.toFixed(4)} | <strong>r² (Determinación):</strong> ${(r2*100).toFixed(2)}%</p>
                    <p><strong>🔮 Pronóstico mes 13:</strong> ${(a + b*13).toFixed(1)} unidades</p>
                    <div class="ia-insight ${ia.clase}"><i class="fas fa-robot"></i> <strong>🤖 IA Analysis:</strong> ${ia.texto}<br><i class="fas fa-lightbulb"></i> <strong>Recomendación:</strong> ${ia.recomendacion}</div>`;
        document.getElementById('resultadoReg').innerHTML = html;

        if (charts.reg) charts.reg.destroy();
        let ctx = document.getElementById('chartReg').getContext('2d');
        let pronosticos = x.map(xi => a + b*xi);
        charts.reg = new Chart(ctx, {
            type: 'scatter',
            plugins: [{ id:'bgWhite', beforeDraw(c){ const ctx=c.ctx; ctx.save(); ctx.fillStyle='#ffffff'; ctx.fillRect(0,0,c.width,c.height); ctx.restore(); } }],
            data: { datasets: [
                { label: 'Datos reales', data: x.map((xi,i) => ({x:xi, y:datos[i]})), borderColor: '#1a6fa8', backgroundColor: '#1a6fa8', pointRadius: 6 },
                { label: `Regresión: y=${a.toFixed(2)}+${b.toFixed(3)}x`, data: x.map((xi,i) => ({x:xi, y:pronosticos[i]})), type: 'line', borderColor: '#e8a020', backgroundColor:'transparent', pointRadius: 0, fill: false }
            ]},
            options: { plugins: { legend: { labels: { color:'#333' } } }, scales: { x: { ticks:{color:'#333'} }, y: { ticks:{color:'#333'} } } }
        });
    }

    function exportarExcelReg() {
        if (!_datosReg.length) { alert("Primero calcula la Regresión"); return; }
        const n = _datosReg.length;
        const cells = [];
        let r = 0;

        cells.push(ct(0, r++, 'Sistema IA de Planificación - Leonardo Carrasco Ocon'));
        cells.push(ct(0, r++, 'Regresión Lineal'));
        r++;

        // Parámetros a y b en celdas para que las fórmulas los usen
        cells.push(ct(0, r, 'Intercepto (a)')); cells.push(cf(1, r, `INTERCEPT(C${r+4}:C${r+3+n},B${r+4}:B${r+3+n})`, Number(_aReg.toFixed(6))));
        const aRef = `B${r+1}`;
        r++;
        cells.push(ct(0, r, 'Pendiente (b)')); cells.push(cf(1, r, `SLOPE(C${r+3}:C${r+2+n},B${r+3}:B${r+2+n})`, Number(_bReg.toFixed(6))));
        const bRef = `B${r+1}`;
        r++;
        cells.push(ct(0, r, 'Correlación (r)')); cells.push(cf(1, r, `CORREL(C${r+2}:C${r+1+n},B${r+2}:B${r+1+n})`, Number(_rReg.toFixed(6))));
        r++;
        cells.push(ct(0, r, 'Determinación (r²)')); cells.push(cf(1, r, `RSQ(C${r+1}:C${r+n},B${r+1}:B${r+n})`, Number(_r2Reg.toFixed(6))));
        r++;
        r++;

        ['Período (X)','X (ingresado)','Demanda (Y)','Ŷ = a + b·X','Error (Y-Ŷ)','Error²','|Error|'].forEach((h,c) => cells.push(ct(c, r, h)));
        r++;
        const ds = r;

        _datosReg.forEach((d, i) => {
            const rr = r + i;
            const ex = rr + 1;
            cells.push(ct(0, rr, `Mes ${i+1}`));
            cells.push(cn(1, rr, i+1));        // X
            cells.push(cn(2, rr, d));           // Y
            cells.push(cf(3, rr, `${aRef}+${bRef}*B${ex}`, Number((_aReg+_bReg*(i+1)).toFixed(4)))); // Ŷ
            cells.push(cf(4, rr, `C${ex}-D${ex}`, Number((d-(_aReg+_bReg*(i+1))).toFixed(4))));
            cells.push(cf(5, rr, `E${ex}^2`,      Math.pow(d-(_aReg+_bReg*(i+1)),2)));
            cells.push(cf(6, rr, `ABS(E${ex})`,   Math.abs(d-(_aReg+_bReg*(i+1)))));
        });

        r += n;
        r++;
        // Pronóstico siguiente
        cells.push(ct(0, r, `Pronóstico mes ${n+1}`));
        cells.push(cn(1, r, n+1));
        cells.push(cf(2, r, `${aRef}+${bRef}*B${r+1}`, Number((_aReg+_bReg*(n+1)).toFixed(4))));
        r += 2;

        // Totales / resumen
        const yStart = ds+1; const yEnd = ds+n;
        cells.push(ct(0, r, 'Suma Y'));      cells.push(cf(1, r, `SUM(C${yStart}:C${yEnd})`, _datosReg.reduce((a,b)=>a+b,0)));
        r++;
        cells.push(ct(0, r, 'Media Y'));     cells.push(cf(1, r, `AVERAGE(C${yStart}:C${yEnd})`, _datosReg.reduce((a,b)=>a+b,0)/n));
        r++;
        cells.push(ct(0, r, 'DAM'));         cells.push(cf(1, r, `AVERAGE(G${yStart}:G${yEnd})`, Number(_datosReg.map((d,i)=>Math.abs(d-(_aReg+_bReg*(i+1)))).reduce((a,b)=>a+b,0)/n).toFixed(4)));

        const ws = construirHoja(cells, 7, r + 1);
        ws['!cols'] = [20,14,14,20,18,14,14].map(w=>({wch:w}));
        const r1rg = ds + 1;
        const r2rg = ds + n;
        descargarExcelConGrafico('Regresion_Lineal', 'Regresión Lineal', ws, {
            tipo: 'dispersion',
            titulo: 'Regresión Lineal — Demanda vs Período',
            ejeX: 'Período (X)', ejeY: 'Demanda (Y)',
            fromCol: 8, fromRow: 2, toCol: 17, toRow: 24,
            series: [
                { label: 'Datos reales',       xCol: 'B', yCol: 'C', r1: r1rg, r2: r2rg, color: '1A6FA8', isLine: false },
                { label: 'Línea regresión',    xCol: 'B', yCol: 'D', r1: r1rg, r2: r2rg, color: 'E8A020', isLine: true  }
            ]
        });
    }

    // --- PAP ---
    let _papDatos = null;

    function calcularPAP() {
        const demandaStr = document.getElementById('demandaPAP').value.trim();
        if (!demandaStr) { alert('⚠️ Ingresa la proyección de demanda (12 meses separados por comas)'); return; }
        const demandas  = demandaStr.split(',').map(Number);
        if (demandas.length < 2 || demandas.some(isNaN)) { alert('⚠️ La demanda debe tener al menos 2 períodos numéricos separados por comas'); return; }
        const invIni    = parseFloat(document.getElementById('invInicialPAP').value);
        const rsPct     = parseFloat(document.getElementById('rsPAP').value)/100;
        if (isNaN(invIni) || isNaN(rsPct)) { alert('⚠️ Completa todos los campos de parámetros antes de calcular'); return; }
        const diasLab   = parseFloat(document.getElementById('diasLabPAP').value);
        const hh        = parseFloat(document.getElementById('hhPAP').value);
        const jornada   = parseFloat(document.getElementById('jornadaPAP').value);
        const costoH    = parseFloat(document.getElementById('costoHoraPAP').value);
        const costoHE   = parseFloat(document.getElementById('costoHoraExtraPAP').value);
        const costoMant = parseFloat(document.getElementById('costoMantPAP').value);
        const costoFalt = parseFloat(document.getElementById('costoFaltPAP').value);
        const costoSub  = parseFloat(document.getElementById('costoSubPAP').value);
        const costoCont = parseFloat(document.getElementById('costoContPAP').value);
        const costoDes  = parseFloat(document.getElementById('costoDesPAP').value);
        const n = demandas.length;
        const meses = ['Ene','Feb','Mar','Abr','May','Jun','Jul','Ago','Sep','Oct','Nov','Dic'];

        // Paso 1: Requerimientos de producción
        const rs   = demandas.map(d => d * rsPct);
        const invI = [invIni]; // inventario inicial de cada mes
        const reqP = []; // requerimiento producción
        const invF = []; // inventario final
        for(let i=0; i<n; i++) {
            const req = Math.round(demandas[i] + rs[i] - invI[i]);
            reqP.push(req);
            const ifin = invI[i] + req - demandas[i];
            invF.push(ifin);
            if(i < n-1) invI.push(ifin);
        }
        const totalReq = reqP.reduce((a,b)=>a+b,0);

        // Horas disponibles por trabajador/mes
        const hDisp = diasLab * jornada; // 176 h/mes por trabajador
        const costoLineal = (w) => w * hDisp * costoH; // costo normal de w trabajadores

        // ── PLAN 1: Persecución ──────────────────────────────────────────
        const hReq1   = reqP.map(r => r * hh);
        const trab1   = hReq1.map(h => Math.ceil(h / hDisp));
        const trabBase = trab1[0];
        const contrat1 = [0], desped1 = [0];
        for(let i=1; i<n; i++){
            const diff = trab1[i] - trab1[i-1];
            contrat1.push(diff > 0 ? diff : 0);
            desped1.push(diff < 0 ? -diff : 0);
        }
        const costoContrat1 = contrat1.map(c => c * costoCont);
        const costoDespid1  = desped1.map(d => d * costoDes);
        // Costo lineal Plan1 = horas requeridas × costo/hora (igual que Excel)
        const costoLin1     = hReq1.map(h => h * costoH);
        const CT1 = costoContrat1.reduce((a,b)=>a+b,0) + costoDespid1.reduce((a,b)=>a+b,0) + costoLin1.reduce((a,b)=>a+b,0);

        // ── PLAN 2: Nivelación — inventario variable con penalidad ────────
        // promTrab = promedio EXACTO de trabajadores Plan1 (sin redondear)
        // Horas disponibles = promTrab × hDisp → prodNiv = horasDisp / hh
        // costoLin = promTrab × hDisp × costoH/mes  (igual que Excel)
        const promTrab       = trab1.reduce((a,b)=>a+b,0) / n;   // exacto (ej: 4.25)
        const horasNivMes    = promTrab * hDisp;                   // horas disponibles/mes
        const prodNiv        = horasNivMes / hh;                   // pares/mes constantes
        const costoLinNivMes = horasNivMes * costoH;               // costo lineal/mes
        const invF2 = [], invSob2 = [], invFalt2 = [];
        let invAct2 = invIni;
        for(let i=0; i<n; i++){
            const ifin = invAct2 + prodNiv - demandas[i];
            invF2.push(ifin);
            const sob = Math.max(0, ifin - rs[i]);
            const falt = Math.max(0, rs[i] - ifin);
            invSob2.push(sob); invFalt2.push(falt);
            invAct2 = ifin;
        }
        const costoInvSob2  = invSob2.map(s => s * costoMant);
        const costoInvFalt2 = invFalt2.map(f => f * costoFalt);
        const costoLin2     = Array(n).fill(costoLinNivMes);
        const CT2 = costoLin2.reduce((a,b)=>a+b,0) + costoInvSob2.reduce((a,b)=>a+b,0) + costoInvFalt2.reduce((a,b)=>a+b,0);

        // ── PLAN 3: Subcontratación ───────────────────────────────────────
        // Misma nivelación, cuando falta se subcontrata
        const invF3 = [], subcontr3 = [];
        let invAct3 = invIni;
        for(let i=0; i<n; i++){
            let ifin = invAct3 + prodNiv - demandas[i];
            let sub = 0;
            if(ifin < rs[i]){ sub = Math.ceil(rs[i] - ifin); ifin += sub; }
            invF3.push(ifin); subcontr3.push(sub);
            invAct3 = ifin;
        }
        const costoInvSob3  = invF3.map((f,i) => Math.max(0, f - rs[i]) * costoMant);
        const costoSub3     = subcontr3.map(s => s * costoSub);
        const costoLin3     = costoLin2.slice();
        const CT3 = costoLin3.reduce((a,b)=>a+b,0) + costoInvSob3.reduce((a,b)=>a+b,0) + costoSub3.reduce((a,b)=>a+b,0);

        // ── PLAN 4: Tiempo Extra ──────────────────────────────────────────
        const invF4 = [], textra4 = [];
        let invAct4 = invIni;
        for(let i=0; i<n; i++){
            let ifin = invAct4 + prodNiv - demandas[i];
            let te = 0;
            if(ifin < rs[i]){ te = Math.ceil(rs[i] - ifin); ifin += te; }
            invF4.push(ifin); textra4.push(te);
            invAct4 = ifin;
        }
        const costoInvSob4 = invF4.map((f,i) => Math.max(0, f - rs[i]) * costoMant);
        const costoTE4     = textra4.map(t => t * hh * costoHE);
        const costoLin4    = costoLin2.slice();
        const CT4 = costoLin4.reduce((a,b)=>a+b,0) + costoInvSob4.reduce((a,b)=>a+b,0) + costoTE4.reduce((a,b)=>a+b,0);

        _papDatos = { demandas, reqP, invF, rs, invI, meses, n,
            p1:{trab:trab1,hReq:hReq1,contrat:contrat1,desped:desped1,costoContrat:costoContrat1,costoDespid:costoDespid1,costoLin:costoLin1,CT:CT1},
            p2:{prod:prodNiv,trab:promTrab,invF:invF2,invSob:invSob2,invFalt:invFalt2,costoSob:costoInvSob2,costoFalt:costoInvFalt2,costoLin:costoLin2,CT:CT2},
            p3:{prod:prodNiv,trab:promTrab,invF:invF3,sub:subcontr3,costoSob:costoInvSob3,costoSub:costoSub3,costoLin:costoLin3,CT:CT3},
            p4:{prod:prodNiv,trab:promTrab,invF:invF4,te:textra4,costoSob:costoInvSob4,costoTE:costoTE4,costoLin:costoLin4,CT:CT4},
            params:{invIni,rsPct,diasLab,hh,jornada,costoH,costoHE,costoMant,costoFalt,costoSub,costoCont,costoDes,hDisp,totalReq}
        };

        const planes = [CT1,CT2,CT3,CT4];
        const mejorPlan = planes.indexOf(Math.min(...planes)) + 1;

        const th = (txt) => `<th style="background:#10323e;color:#a5f3fc;padding:4px 6px">${txt}</th>`;
        const td = (txt,bold=false) => `<td style="padding:3px 6px;text-align:right;${bold?'color:#00f2fe;font-weight:bold':''}">${txt}</td>`;
        const tl = (txt) => `<td style="padding:3px 6px;text-align:left">${txt}</td>`;
        const fmtC = v => `S/ ${v.toLocaleString('es-PE',{minimumFractionDigits:2,maximumFractionDigits:2})}`;
        const fmtN = v => typeof v === 'number' ? v.toFixed(1) : v;

        const mkTabla = (titulo, filas, costoTotal, color='#10323e') =>
            `<div style="margin-bottom:1rem">
            <p style="font-weight:700;color:#00f2fe;margin-bottom:4px">${titulo}</p>
            <div style="overflow-x:auto"><table style="width:100%;border-collapse:collapse;font-size:0.75rem">
            <thead><tr>${th('Concepto')}${meses.map(m=>th(m)).join('')}${th('Total')}</tr></thead>
            <tbody>${filas}</tbody></table></div>
            <p style="text-align:right;margin-top:4px"><strong>Costo Total: ${fmtC(costoTotal)}</strong> | Costo/par: <strong>${fmtC(costoTotal/totalReq)}</strong></p></div>`;

        // sinTotal=true → muestra "—" en la columna Total (filas de promedios/tasas)
        const fila = (label, vals, fmt=(v=>fmtN(v)), bold=false, sinTotal=false) => {
            const tot = vals.reduce((a,b)=>a+(typeof b==='number'?b:0),0);
            const totalCell = sinTotal ? td('—') : td(fmt(tot), bold);
            return `<tr>${tl(label)}${vals.map(v=>td(fmt(v),bold)).join('')}${totalCell}</tr>`;
        };

        // Paso 1 tabla
        let f1 = '';
        f1 += fila('Requerimiento producción (pares)', reqP, v=>Math.round(v));
        f1 += fila('Horas requeridas',                 hReq1, v=>v.toFixed(0));
        f1 += fila('Días de trabajo por mes',           Array(n).fill(diasLab), v=>v, false, true);
        f1 += fila('Horas por mes por trabajador',      Array(n).fill(hDisp), v=>v, false, true);
        f1 += fila('Trabajadores requeridos',           trab1, v=>v, false, true);
        f1 += fila('Nuevos contratados',                contrat1, v=>v);
        f1 += fila('Costo contratación (S/.)',          costoContrat1, fmtC);
        f1 += fila('Trabajadores despedidos',           desped1, v=>v);
        f1 += fila('Costo despido (S/.)',               costoDespid1, fmtC);
        f1 += fila('Costo lineal (S/.) = HH × S/./h',  costoLin1, fmtC, true);

        // Nota informativa Plan 1
        f1 += `<tr><td colspan="${n+2}" style="font-size:0.72rem;color:#8bb3cc;padding:3px 6px">
            Promedio trabajadores Plan1: <strong>${promTrab.toFixed(4)}</strong> → Horas niveladas/mes: <strong>${horasNivMes.toFixed(0)}</strong> →
            Producción nivelada base Planes 2/3/4: <strong>${prodNiv.toFixed(2)}</strong> pares/mes |
            Costo lineal nivelado/mes: <strong>${fmtC(costoLinNivMes)}</strong>
        </td></tr>`;

        // Paso 2 tabla
        let f2 = '';
        f2 += fila('Producción constante (pares)',      Array(n).fill(prodNiv), v=>v.toFixed(2), false, true);
        f2 += fila('Inventario final (pares)',          invF2, v=>v.toFixed(1), false, true);
        f2 += fila('Unidades sobrantes (pares)',        invSob2, v=>v.toFixed(1));
        f2 += fila('Costo inventario sobrante (S/.)',   costoInvSob2, fmtC);
        f2 += fila('Costo lineal (S/.)',                costoLin2, fmtC, true);

        // Paso 3 tabla
        let f3 = '';
        f3 += fila('Producción normal (pares)',         Array(n).fill(prodNiv), v=>v.toFixed(2), false, true);
        f3 += fila('Subcontratado (pares)',             subcontr3, v=>v);
        f3 += fila('Costo subcontratación (S/.)',       costoSub3, fmtC);
        f3 += fila('Inventario sobrante (pares)',       invF3.map((f,i)=>Math.max(0,f-rs[i])), v=>v.toFixed(1), false, true);
        f3 += fila('Costo inventario sobrante (S/.)',   costoInvSob3, fmtC);
        f3 += fila('Costo lineal (S/.)',                costoLin3, fmtC, true);

        // Paso 4 tabla
        let f4 = '';
        f4 += fila('Producción normal (pares)',         Array(n).fill(prodNiv), v=>v.toFixed(2), false, true);
        f4 += fila('Tiempo extra (pares)',              textra4, v=>v);
        f4 += fila('Costo tiempo extra (S/.)',          costoTE4, fmtC);
        f4 += fila('Inventario sobrante (pares)',       invF4.map((f,i)=>Math.max(0,f-rs[i])), v=>v.toFixed(1), false, true);
        f4 += fila('Costo inventario sobrante (S/.)',   costoInvSob4, fmtC);
        f4 += fila('Costo lineal (S/.)',                costoLin4, fmtC, true);

        const ia = interpretacionIA('pap', { costo: Math.min(...planes) });
        const resumen = `
        <div class="ia-insight success" style="margin-bottom:1rem">
        <strong>🏆 Plan seleccionado: Plan ${mejorPlan}</strong> — Menor costo total: ${fmtC(planes[mejorPlan-1])}<br>
        ${ia.texto} ${ia.recomendacion}
        </div>
        <table style="width:auto;font-size:0.8rem;border-collapse:collapse;margin-bottom:1rem">
        <thead><tr>${th('Costo')}${th('Plan 1 Persecución')}${th('Plan 2 Nivelación')}${th('Plan 3 Subcontr.')}${th('Plan 4 T.Extra')}</tr></thead>
        <tbody>
        <tr>${tl('Contratación')}${td(fmtC(costoContrat1.reduce((a,b)=>a+b,0)))}${td('—')}${td('—')}${td('—')}</tr>
        <tr>${tl('Despido')}${td(fmtC(costoDespid1.reduce((a,b)=>a+b,0)))}${td('—')}${td('—')}${td('—')}</tr>
        <tr>${tl('Inventario')}${td('—')}${td(fmtC(costoInvSob2.reduce((a,b)=>a+b,0)))}${td(fmtC(costoInvSob3.reduce((a,b)=>a+b,0)))}${td(fmtC(costoInvSob4.reduce((a,b)=>a+b,0)))}</tr>
        <tr>${tl('Subcontratación')}${td('—')}${td('—')}${td(fmtC(costoSub3.reduce((a,b)=>a+b,0)))}${td('—')}</tr>
        <tr>${tl('Tiempo extra')}${td('—')}${td('—')}${td('—')}${td(fmtC(costoTE4.reduce((a,b)=>a+b,0)))}</tr>
        <tr>${tl('Costo lineal')}${[costoLin1,costoLin2,costoLin3,costoLin4].map(cl=>td(fmtC(cl.reduce((a,b)=>a+b,0)))).join('')}</tr>
        <tr style="background:#0e2a33">${tl('<strong>TOTAL</strong>')}${planes.map((p,i)=>td(fmtC(p),i===mejorPlan-1)).join('')}</tr>
        <tr>${tl('S/. por par')}${planes.map((p,i)=>td(fmtC(p/totalReq),i===mejorPlan-1)).join('')}</tr>
        </tbody></table>`;

        document.getElementById('resultadoPAP').innerHTML =
            resumen +
            mkTabla('📋 Plan 1 — Persecución (fuerza laboral variable)', f1, CT1) +
            mkTabla('📋 Plan 2 — Nivelación (inventario variable, penalidad)', f2, CT2) +
            mkTabla('📋 Plan 3 — Nivelación + Subcontratación', f3, CT3) +
            mkTabla('📋 Plan 4 — Nivelación + Tiempo Extra', f4, CT4);

        // Gráfico PAP — barras comparativas de costos + línea demanda
        if (charts.pap) charts.pap.destroy();
        const ctxPAP = document.getElementById('chartPAP').getContext('2d');
        const bgPAP = [{ id:'bgW', beforeDraw(c){const x=c.ctx;x.save();x.fillStyle='#ffffff';x.fillRect(0,0,c.width,c.height);x.restore();}}];
        charts.pap = new Chart(ctxPAP, {
            type: 'bar',
            plugins: bgPAP,
            data: {
                labels: meses,
                datasets: [
                    {
                        label: 'Demanda (pares)',
                        data: demandas,
                        type: 'line',
                        borderColor: '#1A6FA8',
                        backgroundColor: 'rgba(26,111,168,0.1)',
                        borderWidth: 2,
                        pointBackgroundColor: '#1A6FA8',
                        yAxisID: 'y',
                        order: 0
                    },
                    {
                        label: 'Plan 1 Persecución — Prod.',
                        data: p1.trab.map((w,i) => w * hDisp / hh),
                        backgroundColor: 'rgba(232,160,32,0.7)',
                        yAxisID: 'y',
                        order: 1
                    },
                    {
                        label: 'Plan 2 Nivelación — Prod.',
                        data: Array(n).fill(p2.prod),
                        backgroundColor: 'rgba(74,222,128,0.7)',
                        yAxisID: 'y',
                        order: 2
                    },
                    {
                        label: 'Costo P1 (S/.)',
                        data: p1.costoLin.map((c,i)=>c+p1.costoContrat[i]+p1.costoDespid[i]),
                        backgroundColor: 'rgba(248,113,113,0.6)',
                        yAxisID: 'y2',
                        order: 3
                    },
                    {
                        label: 'Costo P2 (S/.)',
                        data: p2.costoLin.map((c,i)=>c+p2.costoSob[i]+p2.costoFalt[i]),
                        backgroundColor: 'rgba(192,132,252,0.6)',
                        yAxisID: 'y2',
                        order: 4
                    }
                ]
            },
            options: {
                responsive: true,
                interaction: { mode: 'index', intersect: false },
                plugins: {
                    legend: { labels: { color:'#333', font:{size:11} } },
                    title: { display: true, text: 'PAP — Demanda, Producción y Costos por Mes', color:'#333', font:{size:13,weight:'bold'} }
                },
                scales: {
                    x: { ticks:{color:'#333'}, grid:{color:'#eee'} },
                    y: { position:'left', ticks:{color:'#1A6FA8'}, title:{display:true,text:'Pares',color:'#1A6FA8'}, grid:{color:'#eee'} },
                    y2:{ position:'right', ticks:{color:'#883c2c'}, title:{display:true,text:'Costo (S/.)',color:'#883c2c'}, grid:{drawOnChartArea:false} }
                }
            }
        });
    }

    function exportarExcelPAP() {
        if (!_papDatos) { alert("Primero calcula el PAP"); return; }
        const { demandas, meses, n, reqP,
                p1, p2, p3, p4,
                params } = _papDatos;
        const { invIni, rsPct, diasLab, hh, jornada,
                costoH, costoHE, costoMant, costoFalt,
                costoSub, costoCont, costoDes, hDisp, totalReq } = params;

        const fmtC = v => v.toFixed(2);
        const wb = XLSX.utils.book_new();

        // ── Función para generar una hoja por plan ──────────────────────
        function hojaResumen() {
            const cells = [];
            let r = 0;
            cells.push(ct(0, r++, 'Sistema IA de Planificación - Leonardo Carrasco Ocon'));
            cells.push(ct(0, r++, 'Plan Agregado de Producción (PAP) — Resumen Comparativo'));
            r++;

            // Parámetros
            const params2 = [
                ['Inv. inicial (pares)', invIni],
                ['Reserva seguridad (%)', rsPct*100],
                ['Días laborables/mes', diasLab],
                ['HH requeridas/par', hh],
                ['Jornada diaria (h)', jornada],
                ['Horas disponibles/trab./mes', hDisp],
                ['Costo lineal (S/./h)', costoH],
                ['Costo T.Extra (S/./h)', costoHE],
                ['Costo mantener inv. (S/./par/mes)', costoMant],
                ['Costo faltante (S/./par/mes)', costoFalt],
                ['Costo subcontratación (S/./par)', costoSub],
                ['Costo contratación (S/./trab.)', costoCont],
                ['Costo despido (S/./trab.)', costoDes],
            ];
            params2.forEach(([k, v]) => {
                cells.push(ct(0, r, k));
                cells.push(cn(1, r, v));
                r++;
            });
            r++;

            // Tabla comparativa
            const planes = ['Plan 1 Persecución', 'Plan 2 Nivelación', 'Plan 3 Subcontratación', 'Plan 4 Tiempo Extra'];
            const cts    = [p1.CT, p2.CT, p3.CT, p4.CT];
            ['Concepto', ...planes, 'Mejor Plan'].forEach((h,c) => cells.push(ct(c, r, h)));
            r++;

            const conceptos = [
                ['Costo contratación (S/.)',    [p1.costoContrat.reduce((a,b)=>a+b,0), 0, 0, 0]],
                ['Costo despido (S/.)',         [p1.costoDespid.reduce((a,b)=>a+b,0), 0, 0, 0]],
                ['Costo inventario sobrante (S/.)', [0, p2.costoSob.reduce((a,b)=>a+b,0), p3.costoSob.reduce((a,b)=>a+b,0), p4.costoSob.reduce((a,b)=>a+b,0)]],
                ['Costo subcontratación (S/.)', [0, 0, p3.costoSub.reduce((a,b)=>a+b,0), 0]],
                ['Costo tiempo extra (S/.)',    [0, 0, 0, p4.costoTE.reduce((a,b)=>a+b,0)]],
                ['Costo lineal total (S/.)',    [p1.costoLin.reduce((a,b)=>a+b,0), p2.costoLin.reduce((a,b)=>a+b,0), p3.costoLin.reduce((a,b)=>a+b,0), p4.costoLin.reduce((a,b)=>a+b,0)]],
                ['COSTO TOTAL (S/.)',           cts],
                ['S/. por par',                cts.map(c=>c/totalReq)],
            ];
            const mejorIdx = cts.indexOf(Math.min(...cts));
            conceptos.forEach(([label, vals]) => {
                cells.push(ct(0, r, label));
                vals.forEach((v, c) => cells.push(cn(c+1, r, Number(v.toFixed(2)))));
                cells.push(ct(5, r, planes[mejorIdx]));
                r++;
            });

            r++;
            cells.push(ct(0, r, `Total requerimiento producción (pares)`));
            cells.push(cn(1, r, totalReq));

            const ws = construirHoja(cells, 6, r+1);
            ws['!cols'] = [38,18,18,18,18,20].map(w=>({wch:w}));
            XLSX.utils.book_append_sheet(wb, ws, 'Resumen');
        }

        // ── Hoja por plan ────────────────────────────────────────────────
        function hojaDetalle(nombre, planDatos, filasDef) {
            const cells = [];
            let r = 0;
            cells.push(ct(0, r++, `PAP — ${nombre}`));
            r++;

            // Encabezados
            ['Concepto', ...meses, 'Total'].forEach((h,c) => cells.push(ct(c, r, h)));
            r++;
            const ds = r;

            filasDef.forEach(([label, vals]) => {
                cells.push(ct(0, r, label));
                const tot = vals.reduce((a,b)=>a+(typeof b==='number'?b:0), 0);
                vals.forEach((v, c) => {
                    if (typeof v === 'number') cells.push(cn(c+1, r, Number(v.toFixed(4))));
                    else cells.push(ct(c+1, r, v));
                });
                cells.push(cn(n+1, r, Number(tot.toFixed(4))));
                r++;
            });

            const ws = construirHoja(cells, n+2, r);
            ws['!cols'] = [36, ...Array(n).fill(11), 12].map(w=>({wch:w}));
            XLSX.utils.book_append_sheet(wb, ws, nombre.substring(0,31));
        }

        hojaResumen();

        hojaDetalle('Plan1 Persecución', p1, [
            ['Demanda (pares)',             demandas],
            ['Requerimiento prod. (pares)', reqP],
            ['Horas requeridas',            p1.trab.map((w,i)=>reqP[i]*hh)],
            ['Trabajadores requeridos',     p1.trab],
            ['Nuevos contratados',          p1.contrat],
            ['Costo contratación (S/.)',    p1.costoContrat],
            ['Trabajadores despedidos',     p1.desped],
            ['Costo despido (S/.)',         p1.costoDespid],
            ['Costo lineal (S/.)',          p1.costoLin],
        ]);

        hojaDetalle('Plan2 Nivelación', p2, [
            ['Demanda (pares)',             demandas],
            ['Producción constante (pares)',Array(n).fill(p2.prod)],
            ['Inventario final (pares)',    p2.invF],
            ['Unidades sobrantes (pares)',  p2.invSob],
            ['Costo inv. sobrante (S/.)',   p2.costoSob],
            ['Costo inv. faltante (S/.)',   p2.costoFalt],
            ['Costo lineal (S/.)',          p2.costoLin],
        ]);

        hojaDetalle('Plan3 Subcontratación', p3, [
            ['Demanda (pares)',             demandas],
            ['Producción normal (pares)',   Array(n).fill(p3.prod)],
            ['Subcontratado (pares)',       p3.sub],
            ['Costo subcontratación (S/.)', p3.costoSub],
            ['Inventario sobrante (pares)', p3.invF.map((f,i)=>Math.max(0,f-demandas[i]*_papDatos.params.rsPct))],
            ['Costo inv. sobrante (S/.)',   p3.costoSob],
            ['Costo lineal (S/.)',          p3.costoLin],
        ]);

        hojaDetalle('Plan4 Tiempo Extra', p4, [
            ['Demanda (pares)',             demandas],
            ['Producción normal (pares)',   Array(n).fill(p4.prod)],
            ['Tiempo extra (pares)',        p4.te],
            ['Costo tiempo extra (S/.)',    p4.costoTE],
            ['Inventario sobrante (pares)', p4.invF.map((f,i)=>Math.max(0,f-demandas[i]*_papDatos.params.rsPct))],
            ['Costo inv. sobrante (S/.)',   p4.costoSob],
            ['Costo lineal (S/.)',          p4.costoLin],
        ]);

        XLSX.writeFile(wb, 'PAP_Plan_Agregado.xlsx');
    }

    // --- PMP ---
    let _pmpDatos = null;

    function calcularPMP() {
        const reqTotal = parseFloat(document.getElementById('reqProdPAP').value);
        const diasLab  = parseFloat(document.getElementById('diasLab').value);
        const loteMin  = parseFloat(document.getElementById('loteMin').value);
        if (isNaN(reqTotal) || isNaN(diasLab) || isNaN(loteMin)) {
            alert('⚠️ Completa los campos: Req. producción, Días laborables y Lote mínimo');
            return;
        }

        // Leer datos dinámicos desde pmpSkuData
        if (!pmpSkuData || pmpSkuData.length === 0) {
            alert('⚠️ Primero presiona "Recargar desde BOM" para cargar los SKUs');
            return;
        }

        // Leer valores actuales de los inputs dinámicos
        pmpSkuData.forEach((sku, i) => {
            sku.ventas = parseFloat(document.getElementById(`pmp_ventas_${i}`)?.value) || 0;
            sku.invIni = parseFloat(document.getElementById(`pmp_invini_${i}`)?.value) || 0;
            sku.ss     = parseFloat(document.getElementById(`pmp_ss_${i}`)?.value)     || 0;
        });

        const ventas  = pmpSkuData.map(s => s.ventas);
        const invIni  = pmpSkuData.map(s => s.invIni);
        const ss      = pmpSkuData.map(s => s.ss);
        const skuNom  = pmpSkuData.map(s => s.prod);

        if (ventas.every(v => v === 0)) { alert('⚠️ Ingresa las ventas previas de al menos un SKU'); return; }


        const totalVentas = ventas.reduce((a,b)=>a+b,0);
        const pct  = ventas.map(v => v / totalVentas);              // % participación
        const pron = pct.map(p => p * reqTotal);                    // pronóstico en pares
        const cantProd = pron.map((p,i) => Math.max(0, p + ss[i] - invIni[i])); // cant a producir
        const nLotes   = cantProd.map(c => Math.ceil(c / 12));      // nº lotes (docenas de 12 pares)

        // Explosión semanal (4 semanas iguales)
        const semanal  = cantProd.map(c => c / 4);

        _pmpDatos = { pron, cantProd, nLotes, semanal, loteMin, diasLab, pct, ventas, invIni, ss, skuNom, reqTotal };

        const th = t => `<th style="background:#10323e;color:#a5f3fc;padding:4px 6px">${t}</th>`;
        const td = v => `<td style="padding:3px 6px;text-align:right">${typeof v==='number'?v.toFixed(2):v}</td>`;
        const tl = v => `<td style="padding:3px 6px;text-align:left">${v}</td>`;

        let filas = skuNom.map((nom,i) =>
            `<tr>${tl(nom)}${td(ventas[i])}${td((pct[i]*100).toFixed(2)+'%')}${td(pron[i])}${td(ss[i])}${td(invIni[i])}${td(cantProd[i])}${td(12)}${td(nLotes[i])}</tr>`
        ).join('');
        const totV = ventas.reduce((a,b)=>a+b,0);
        const totPron = pron.reduce((a,b)=>a+b,0);
        const totCant = cantProd.reduce((a,b)=>a+b,0);
        filas += `<tr style="font-weight:bold;background:#0e2a33"><td>TOTAL</td>${td(totV)}${td('100%')}${td(totPron)}${td('')}${td('')}${td(totCant)}${td('')}${td(nLotes.reduce((a,b)=>a+b,0))}</tr>`;

        let semanFil = skuNom.map((nom,i) =>
            `<tr>${tl(nom)}${[1,2,3,4].map(()=>td(semanal[i])).join('')}${td(cantProd[i])}</tr>`
        ).join('');

        const html2 = `
        <p style="font-weight:700;color:#00f2fe;margin-bottom:6px">a) PMP Mensual — Enero (Mes 1)</p>
        <div style="overflow-x:auto"><table style="width:100%;border-collapse:collapse;font-size:0.75rem">
        <thead><tr>${['Producto','Ventas prev.','% Partic.','Pronóstico (pares)','SS (pares)','Inv.Ini (pares)','Cant. Producir','Vol/Fórmula','Nº Lotes'].map(th).join('')}</tr></thead>
        <tbody>${filas}</tbody></table></div>

        <p style="font-weight:700;color:#00f2fe;margin:1rem 0 6px">b) PMP Semanal — Producción igual S1=S2=S3=S4</p>
        <div style="overflow-x:auto"><table style="width:100%;border-collapse:collapse;font-size:0.75rem">
        <thead><tr>${['Producto','S1','S2','S3','S4','Total'].map(th).join('')}</tr></thead>
        <tbody>${semanFil}</tbody></table></div>

        <p style="margin-top:0.5rem"><strong>Total a producir en Enero:</strong> ${totCant.toFixed(2)} pares &nbsp;|&nbsp;
        <strong>Producción/corrida:</strong> ${(totCant/diasLab).toFixed(2)} pares/día</p>`;
        document.getElementById('resultadoPMP').innerHTML = html2;
        generarOrdenesAprovisionamiento();

        // Gráfico PMP — barras por SKU (participación) + línea cant. producir
        if (charts.pmp) charts.pmp.destroy();
        const ctxPMP = document.getElementById('chartPMP').getContext('2d');
        const bgPMP = [{ id:'bgW', beforeDraw(c){const x=c.ctx;x.save();x.fillStyle='#ffffff';x.fillRect(0,0,c.width,c.height);x.restore();}}];
        const colorsSKU = ['rgba(26,111,168,0.8)','rgba(232,160,32,0.8)','rgba(74,222,128,0.8)','rgba(248,113,113,0.8)'];
        charts.pmp = new Chart(ctxPMP, {
            type: 'bar',
            plugins: bgPMP,
            data: {
                labels: skuNom.map(s => s.replace('SKU','').trim()),
                datasets: [
                    {
                        label: 'Pronóstico (pares)',
                        data: pron,
                        backgroundColor: colorsSKU,
                        borderColor: colorsSKU.map(c=>c.replace('0.8','1')),
                        borderWidth: 1,
                        yAxisID: 'y'
                    },
                    {
                        label: 'Cant. a Producir (pares)',
                        data: cantProd,
                        type: 'line',
                        borderColor: '#1A6FA8',
                        backgroundColor: 'rgba(26,111,168,0.15)',
                        borderWidth: 2,
                        pointBackgroundColor: '#1A6FA8',
                        pointRadius: 6,
                        yAxisID: 'y'
                    },
                    {
                        label: '% Participación',
                        data: pct.map(p => p*100),
                        type: 'line',
                        borderColor: '#E8A020',
                        borderDash: [5,4],
                        borderWidth: 2,
                        pointBackgroundColor: '#E8A020',
                        pointRadius: 5,
                        yAxisID: 'y2'
                    }
                ]
            },
            options: {
                responsive: true,
                plugins: {
                    legend: { labels: { color:'#333', font:{size:11} } },
                    title: { display: true, text: 'PMP — Pronóstico y Producción por SKU', color:'#333', font:{size:13,weight:'bold'} }
                },
                scales: {
                    x: { ticks:{color:'#333'}, grid:{color:'#eee'} },
                    y: { position:'left', ticks:{color:'#1A6FA8'}, title:{display:true,text:'Pares',color:'#1A6FA8'}, grid:{color:'#eee'} },
                    y2:{ position:'right', ticks:{color:'#E8A020',callback:v=>v.toFixed(1)+'%'}, title:{display:true,text:'% Partic.',color:'#E8A020'}, grid:{drawOnChartArea:false} }
                }
            }
        });
    }

    function exportarExcelPMP() {
        if (!_pmpDatos) { alert("Primero calcula el PMP"); return; }
        const { pron, cantProd, nLotes, semanal, loteMin, invIni, ss, ventas, skuNom, reqTotal } = _pmpDatos;
        const n = skuNom.length;
        const cells = [];
        let r = 0;

        cells.push(ct(0, r++, 'Sistema IA de Planificación - Leonardo Carrasco Ocon'));
        cells.push(ct(0, r++, 'Plan Maestro de Producción (PMP) — Enero'));
        r++;

        // Encabezados tabla mensual
        ['Producto','Ventas prev.','% Partic.','Pronóstico (pares)','SS (pares)','Inv.Ini (pares)','Cant. Producir','Vol/Fórmula (pares)','Nº Lotes']
            .forEach((h,c) => cells.push(ct(c, r, h)));
        r++;
        const ds = r;

        const totV = ventas.reduce((a,b)=>a+b,0);
        skuNom.forEach((nom, i) => {
            cells.push(ct(0, r+i, nom));
            cells.push(cn(1, r+i, ventas[i]));
            // % participación con fórmula
            const vCell = `B${ds+i+1}`;
            const totVCell = `B${ds+n+1}`; // fila total ventas
            cells.push(cf(2, r+i, `${vCell}/SUM(B${ds+1}:B${ds+n})`, Number((_pmpDatos.pct[i]).toFixed(6))));
            cells.push(cn(3, r+i, Number(pron[i].toFixed(4))));
            cells.push(cn(4, r+i, ss[i]));
            cells.push(cn(5, r+i, invIni[i]));
            // Cant producir = MAX(0, Pron+SS-InvIni)
            cells.push(cf(6, r+i, `MAX(0,D${ds+i+1}+E${ds+i+1}-F${ds+i+1})`, Number(cantProd[i].toFixed(4))));
            cells.push(cn(7, r+i, 12)); // vol por fórmula = 12 pares/docena
            // Nº lotes = CEILING(cant/12)
            cells.push(cf(8, r+i, `CEILING(G${ds+i+1}/12,1)`, nLotes[i]));
        });
        r += n;

        // Fila total
        cells.push(ct(0, r, 'TOTAL'));
        cells.push(cf(1, r, `SUM(B${ds+1}:B${ds+n})`, totV));
        cells.push(ct(2, r, '100%'));
        cells.push(cf(3, r, `SUM(D${ds+1}:D${ds+n})`, pron.reduce((a,b)=>a+b,0)));
        cells.push(ct(4, r, '')); cells.push(ct(5, r, ''));
        cells.push(cf(6, r, `SUM(G${ds+1}:G${ds+n})`, cantProd.reduce((a,b)=>a+b,0)));
        cells.push(ct(7, r, ''));
        cells.push(cf(8, r, `SUM(I${ds+1}:I${ds+n})`, nLotes.reduce((a,b)=>a+b,0)));
        r += 2;

        // Tabla semanal
        cells.push(ct(0, r++, 'PMP Semanal — Producción igual S1=S2=S3=S4'));
        ['Producto','S1','S2','S3','S4','Total'].forEach((h,c) => cells.push(ct(c, r, h)));
        r++;
        const ss2 = r;
        skuNom.forEach((nom, i) => {
            cells.push(ct(0, r+i, nom));
            [1,2,3,4].forEach((_, s) => cells.push(cn(s+1, r+i, Number(semanal[i].toFixed(4)))));
            cells.push(cf(5, r+i, `SUM(B${ss2+i+1}:E${ss2+i+1})`, Number(cantProd[i].toFixed(4))));
        });

        const ws = construirHoja(cells, 9, r + n + 1);
        ws['!cols'] = [34,12,12,16,12,12,16,14,12].map(w=>({wch:w}));
        descargarExcel('PMP_Plan_Maestro', 'PMP', ws);
    }

    // --- MRP ---
    let _mrpDatos = null;

    // ── MRP — helpers de UI ────────────────────────────────────────────────
    // Lee los inputs de la tabla de inventarios y actualiza inventariosData en memoria
    // Se llama automáticamente antes de cualquier operación que dependa de inventarios
    function sincronizarInventarios() {
        const n = inventariosData.length;
        for (let i = 0; i < n; i++) {
            const matEl   = document.getElementById(`mat_${i}`);
            const stockEl = document.getElementById(`stock_${i}`);
            const loteEl  = document.getElementById(`lote_${i}`);
            const ltEl    = document.getElementById(`lt_${i}`);
            if (matEl)   inventariosData[i].material = matEl.value.trim();
            if (stockEl) inventariosData[i].stock    = parseFloat(stockEl.value) || 0;
            if (loteEl)  inventariosData[i].lote     = loteEl.value.trim();
            if (ltEl)    inventariosData[i].lt        = parseFloat(ltEl.value) || 0;
        }
    }

    function poblarSelectMRP() {
        const sel = document.getElementById('materialMRP');
        if (!sel) return;
        const prevVal = sel.value;
        sel.innerHTML = '';
        inventariosData.forEach(item => {
            const opt = document.createElement('option');
            opt.value = item.material;
            opt.textContent = item.material;
            sel.appendChild(opt);
        });
        // Restaurar selección anterior si sigue existiendo
        if (prevVal && inventariosData.find(i => i.material === prevVal)) {
            sel.value = prevVal;
        }
        actualizarMaterialMRP();
    }

    function actualizarMaterialMRP() {
        sincronizarInventarios(); // asegurar que inventariosData está al día
        const sel = document.getElementById('materialMRP');
        if (!sel) return;
        const mat = sel.value;
        const inv = inventariosData.find(i => i.material === mat);
        const el  = document.getElementById('infoMaterialMRP');
        if (!el) return;
        if (inv) {
            el.innerHTML = `
                <strong style="color:#00f2fe">${inv.material}</strong><br>
                📦 Stock inicial: <strong>${inv.stock}</strong> ${inv.und}
                &nbsp;|&nbsp; 📦 Lote: <strong>${inv.lote}</strong>
                &nbsp;|&nbsp; ⏱ Lead Time: <strong>${inv.lt}</strong> período(s)`;
        } else {
            el.innerHTML = '<span style="color:#f87171">Material no encontrado en inventarios. Ve a la pestaña Inventarios y guarda los cambios.</span>';
        }
    }

    function generarInputsMRP() {
        const modo    = document.getElementById('modoMRP').value;
        const nPer    = parseInt(document.getElementById('nPeriodosMRP').value) || 4;
        const nPrev   = parseInt(document.getElementById('periodosPrevMRP').value) || 0;
        const nTotal  = nPrev + nPer;

        const labelPrev = i => modo === 'semanas' ? `S-${nPrev-i}` : `M-${nPrev-i}`;
        const labelAct  = i => modo === 'semanas' ? `S${i+1}` : `M${i+1}`;

        let html2 = `<p style="font-size:0.78rem;color:#8bb3cc;margin-bottom:0.5rem">
            Ingresa las <strong>Necesidades Brutas</strong> por período
            (${modo === 'semanas' ? 'semanas' : 'meses'}).
            Los períodos previos sirven como contexto para el Lead Time (déjalos en 0 si no aplica).
        </p>
        <div style="display:flex;flex-wrap:wrap;gap:0.4rem;align-items:flex-end">`;

        // Períodos previos
        for (let i = 0; i < nPrev; i++) {
            html2 += `<div style="text-align:center;min-width:70px">
                <div style="font-size:0.65rem;color:#facc15;margin-bottom:2px">${labelPrev(i)} (prev)</div>
                <input type="number" id="nb_prev_${i}" value="0" step="any"
                    style="width:70px;text-align:center;background:#1a2f1a;border-color:#3a5c3a">
            </div>`;
        }

        if (nPrev > 0) {
            html2 += `<div style="align-self:center;color:#444;font-size:1.2rem;padding:0 4px">|</div>`;
        }

        // Períodos a planificar
        for (let i = 0; i < nPer; i++) {
            html2 += `<div style="text-align:center;min-width:70px">
                <div style="font-size:0.65rem;color:#00f2fe;margin-bottom:2px">${labelAct(i)}</div>
                <input type="number" id="nb_act_${i}" value="" step="any"
                    placeholder="0" style="width:70px;text-align:center">
            </div>`;
        }
        html2 += `</div>`;

        document.getElementById('contenedorNBMRP').innerHTML = html2;
    }

    function leerNBMRP() {
        const nPrev = parseInt(document.getElementById('periodosPrevMRP').value) || 0;
        const nPer  = parseInt(document.getElementById('nPeriodosMRP').value) || 4;
        const prev  = Array.from({length: nPrev}, (_, i) => parseFloat(document.getElementById(`nb_prev_${i}`)?.value) || 0);
        const act   = Array.from({length: nPer},  (_, i) => parseFloat(document.getElementById(`nb_act_${i}`)?.value)  || 0);
        return { prev, act, nb: [...prev, ...act] };
    }

    // ── MRP — algoritmo principal ───────────────────────────────────────────
    function calcularMRP() {
        sincronizarInventarios(); // leer inputs actuales antes de buscar el material
        poblarSelectMRP();        // re-sincronizar el select por si cambió algo
        const materialSel = document.getElementById('materialMRP').value;
        const modo        = document.getElementById('modoMRP').value;
        const nPer        = parseInt(document.getElementById('nPeriodosMRP').value) || 4;
        const nPrev       = parseInt(document.getElementById('periodosPrevMRP').value) || 0;

        const { nb } = leerNBMRP();
        const nTot = nb.length;

        if (nTot === 0) { alert('⚠️ Genera los campos de NB primero'); return; }

        const inv0     = inventariosData.find(i => i.material === materialSel);
        const stockIni = inv0 ? Number(inv0.stock) : 0;
        const lote     = inv0 ? inv0.lote : 'LFL';
        const lt       = inv0 ? Number(inv0.lt) : 0;

        // ── Algoritmo MRP ──────────────────────────────────────────────────
        const entradas = new Array(nTot).fill(0);
        const stockFin = new Array(nTot).fill(0);
        const nnetas   = new Array(nTot).fill(0);
        const pedidos  = new Array(nTot).fill(0);
        const lanzam   = new Array(nTot).fill(0);

        let stockActual = stockIni;
        for (let t = 0; t < nTot; t++) {
            const disp = stockActual + entradas[t];
            const nn   = nb[t] - disp;
            nnetas[t]  = nn;
            if (nn > 0) {
                let ped = 0;
                const lotN = parseFloat(lote);
                if (lote === 'LFL' || isNaN(lotN) || lotN <= 0) {
                    ped = nn;
                } else {
                    ped = Math.ceil(nn / lotN) * lotN;
                }
                pedidos[t]  = ped;
                entradas[t] += ped;
                // Lanzamiento desplazado lt períodos atrás
                const tLanz = t - lt;
                if (tLanz >= 0) lanzam[tLanz] += ped;
            }
            stockFin[t]  = stockActual + entradas[t] - nb[t];
            stockActual  = stockFin[t];
        }

        _mrpDatos = { nb, entradas, stockFin, nnetas, pedidos, lanzam,
                      nTot, nPrev, nPer, modo, material: materialSel,
                      stockIni, lote, lt };

        // ── Render ─────────────────────────────────────────────────────────
        const labelPrev = i => modo === 'semanas' ? `S-${nPrev-i}` : `M-${nPrev-i}`;
        const labelAct  = i => modo === 'semanas' ? `S${i+1}` : `M${i+1}`;
        const perLabel  = i => i < nPrev ? labelPrev(i) : labelAct(i - nPrev);

        const fv = v => v === 0 ? '—' : (typeof v === 'number' ? v.toFixed(3) : v);
        const fvNN = v => v <= 0 ? '—' : v.toFixed(3);

        const estiloTh = (prev) => prev
            ? 'background:#1a2a1a;color:#facc15;padding:3px 5px;font-size:0.72rem;min-width:65px'
            : 'background:#10323e;color:#a5f3fc;padding:3px 5px;font-size:0.72rem;min-width:65px';
        const estiloCelda = 'padding:3px 5px;text-align:right;font-size:0.75rem';
        const estiloLabel = 'padding:3px 6px;font-size:0.75rem;font-weight:600;white-space:nowrap';

        const mkTh = (i) => `<th style="${estiloTh(i < nPrev)}">${perLabel(i)}</th>`;
        const mkTd = (v, resalt) => `<td style="${estiloCelda}${resalt?';color:#00f2fe;font-weight:bold':''}">${v}</td>`;
        const mkTl = (t, color) => `<td style="${estiloLabel}${color?';color:'+color:''}">${t}</td>`;

        const mkFila = (label, arr, fmt=fv, resalt=false, color='') =>
            `<tr>${mkTl(label, color)}${arr.map((v,i)=>mkTd(fmt(v), resalt && v !== 0)).join('')}
             ${mkTd(arr.reduce((a,b)=>a+(b||0),0).toFixed(3), false)}</tr>`;

        // Separador visual entre previos y activos
        const mkSep = () => nPrev > 0
            ? `<th style="background:#222;width:4px;padding:0"></th>` : '';

        const mkFilaSep = (arr, fmt, resalt, color) => {
            const celdas = arr.map((v,i) => {
                const sep = (i === nPrev && nPrev > 0) ? `<td style="background:#222;width:4px"></td>` : '';
                return sep + mkTd(fmt(v), resalt && v !== 0);
            }).join('');
            return celdas;
        };

        const tot = arr => arr.reduce((a,b)=>a+(b||0),0);

        const ia = interpretacionIA('mrp', { stockFinal: stockFin[nTot-1], lt });

        // Resumen rápido de órdenes de lanzamiento
        const ordenesResumen = lanzam
            .map((v,i) => v > 0 ? `<span style="background:#1a5c2a;padding:2px 8px;border-radius:1rem;margin:2px;display:inline-block;font-size:0.75rem">🚀 ${perLabel(i)}: <strong>${v.toFixed(2)}</strong></span>` : '')
            .filter(Boolean).join('');

        const html2 = `
        <p style="font-size:0.75rem;color:#8bb3cc;margin-bottom:6px">
            <strong style="color:#fff">${materialSel}</strong> &nbsp;|&nbsp;
            Stock ini: <strong>${stockIni}</strong> &nbsp;|&nbsp;
            Lote: <strong>${lote}</strong> &nbsp;|&nbsp;
            LT: <strong>${lt}</strong> período(s) &nbsp;|&nbsp;
            Modo: <strong>${modo}</strong> &nbsp;|&nbsp;
            Stock final: <strong style="color:${stockFin[nTot-1]<0?'#f87171':'#4ade80'}">${stockFin[nTot-1].toFixed(3)}</strong>
        </p>

        <div style="overflow-x:auto;margin-bottom:0.8rem">
        <table style="width:100%;border-collapse:collapse">
        <thead><tr>
            <th style="background:#0a1419;padding:3px 6px;font-size:0.72rem;white-space:nowrap">Concepto</th>
            ${Array.from({length:nTot},(_,i)=>mkTh(i)).join('')}
            ${mkSep()}
            <th style="background:#10323e;color:#a5f3fc;padding:3px 5px;font-size:0.72rem">Total</th>
        </tr></thead>
        <tbody>
        <tr>${mkTl('Necesidades Brutas','#eef2ff')}${mkFilaSep(nb,fv,false,'')}${mkTd(tot(nb).toFixed(3))}</tr>
        <tr>${mkTl('Entradas Previstas','#4ade80')}${mkFilaSep(entradas,fv,false,'')}${mkTd(tot(entradas).toFixed(3))}</tr>
        <tr>${mkTl('Stock Disponible','#a5f3fc')}${mkFilaSep(stockFin,v=>v.toFixed(3),false,'')}${mkTd(stockFin[nTot-1].toFixed(3))}</tr>
        <tr>${mkTl('Necesidades Netas','#facc15')}${mkFilaSep(nnetas,fvNN,false,'')}${mkTd(nnetas.filter(v=>v>0).reduce((a,b)=>a+b,0).toFixed(3))}</tr>
        <tr>${mkTl('Pedidos Planeados','#c084fc')}${mkFilaSep(pedidos,fv,true,'')}${mkTd(tot(pedidos).toFixed(3))}</tr>
        <tr style="background:#0e2a1a">${mkTl('🚀 Lanzamiento Órdenes','#4ade80')}${mkFilaSep(lanzam,fv,true,'')}${mkTd(tot(lanzam).toFixed(3))}</tr>
        </tbody></table></div>

        ${ordenesResumen ? `<p style="margin-bottom:0.5rem"><strong>Órdenes a lanzar:</strong><br>${ordenesResumen}</p>` : '<p style="color:#8bb3cc;font-size:0.8rem">No se generaron órdenes de lanzamiento.</p>'}

        <div class="ia-insight ${ia.clase}">
            <i class="fas fa-robot"></i> <strong>IA:</strong> ${ia.texto}<br>
            <i class="fas fa-lightbulb"></i> ${ia.recomendacion}
        </div>`;

        document.getElementById('resultadoMRP').innerHTML = html2;
        // Mostrar botón "Agregar a Órdenes" después de calcular
        const btnAO = document.getElementById('btnAgregarOrden');
        if (btnAO) btnAO.style.display = 'inline-block';
        generarOrdenesAprovisionamiento();

        // Gráfico MRP — líneas: NB, Stock, Lanzamiento
        if (charts.mrp) charts.mrp.destroy();
        const ctxMRP = document.getElementById('chartMRP').getContext('2d');
        const bgMRP = [{ id:'bgW', beforeDraw(c){const x=c.ctx;x.save();x.fillStyle='#ffffff';x.fillRect(0,0,c.width,c.height);x.restore();}}];
        const labMRP = Array.from({length:nTot},(_,i) => perLabel(i));
        charts.mrp = new Chart(ctxMRP, {
            type: 'line',
            plugins: bgMRP,
            data: {
                labels: labMRP,
                datasets: [
                    {
                        label: 'Necesidades Brutas',
                        data: nb,
                        borderColor: '#1A6FA8',
                        backgroundColor: 'rgba(26,111,168,0.12)',
                        borderWidth: 2,
                        pointBackgroundColor: '#1A6FA8',
                        tension: 0.2,
                        fill: true
                    },
                    {
                        label: 'Stock Disponible',
                        data: stockFin,
                        borderColor: '#4ade80',
                        backgroundColor: 'rgba(74,222,128,0.1)',
                        borderWidth: 2,
                        pointBackgroundColor: '#4ade80',
                        tension: 0.2,
                        fill: true
                    },
                    {
                        label: 'Pedidos Planeados',
                        data: pedidos,
                        borderColor: '#c084fc',
                        backgroundColor: 'rgba(192,132,252,0.15)',
                        borderWidth: 2,
                        borderDash: [4,3],
                        pointBackgroundColor: '#c084fc',
                        pointRadius: v => v.raw > 0 ? 6 : 3,
                        tension: 0
                    },
                    {
                        label: '🚀 Lanzamiento Órdenes',
                        data: lanzam,
                        borderColor: '#E8A020',
                        backgroundColor: 'rgba(232,160,32,0.2)',
                        borderWidth: 2,
                        borderDash: [6,3],
                        pointBackgroundColor: '#E8A020',
                        pointStyle: lanzam.map(v => v > 0 ? 'triangle' : 'circle'),
                        pointRadius: lanzam.map(v => v > 0 ? 8 : 3),
                        tension: 0
                    }
                ]
            },
            options: {
                responsive: true,
                interaction: { mode: 'index', intersect: false },
                plugins: {
                    legend: { labels: { color:'#333', font:{size:11} } },
                    title: { display: true,
                             text: `MRP — ${materialSel} | LT: ${lt} per. | Lote: ${lote}`,
                             color:'#333', font:{size:13,weight:'bold'} },
                    tooltip: {
                        callbacks: {
                            label: ctx => `${ctx.dataset.label}: ${Number(ctx.parsed.y).toFixed(3)}`
                        }
                    }
                },
                scales: {
                    x: { ticks:{color:'#333'}, grid:{color:'#eee'} },
                    y: { ticks:{color:'#333'}, title:{display:true,text:'Unidades',color:'#555'}, grid:{color:'#eee'} }
                }
            }
        });
    }

    // ── exportarExcelMRP ───────────────────────────────────────────────────
    function exportarExcelMRP() {
        if (!_mrpDatos) { alert("Primero calcula el MRP"); return; }
        const { nb, entradas, stockFin, nnetas, pedidos, lanzam,
                nTot, nPrev, nPer, modo, material, stockIni, lote, lt } = _mrpDatos;

        const labelPrev = i => modo === 'semanas' ? `S-${nPrev-i}` : `M-${nPrev-i}`;
        const labelAct  = i => modo === 'semanas' ? `S${i+1}` : `M${i+1}`;
        const perLabel  = i => i < nPrev ? labelPrev(i) : labelAct(i - nPrev);

        const cells = [];
        let r = 0;

        cells.push(ct(0, r++, 'Sistema IA de Planificación - Leonardo Carrasco Ocon'));
        cells.push(ct(0, r++, `MRP — ${material} (${modo})`));
        r++;

        // Parámetros
        cells.push(ct(0, r, 'Material'));          cells.push(ct(1, r++, material));
        cells.push(ct(0, r, 'Stock Inicial'));     cells.push(cn(1, r, stockIni));
        const sIRef = `B${r+1}`; r++;
        cells.push(ct(0, r, 'Tamaño de Lote'));   cells.push(ct(1, r++, String(lote)));
        cells.push(ct(0, r, `Lead Time (${modo === 'semanas' ? 'sem' : 'meses'})`));
        cells.push(cn(1, r++, lt));
        cells.push(ct(0, r, 'Modo'));              cells.push(ct(1, r++, modo));
        cells.push(ct(0, r, 'Períodos previos'));  cells.push(cn(1, r++, nPrev));
        cells.push(ct(0, r, 'Períodos planif.'));  cells.push(cn(1, r++, nPer));
        r++;

        // Encabezados
        cells.push(ct(0, r, 'Concepto'));
        for (let i = 0; i < nTot; i++) cells.push(ct(i+1, r, perLabel(i)));
        cells.push(ct(nTot+1, r, 'Total'));
        r++;

        const mkFila = (label, arr) => {
            cells.push(ct(0, r, label));
            arr.forEach((v, i) => cells.push(cn(i+1, r, Number(v.toFixed ? v.toFixed(6) : v))));
            const tot = arr.reduce((a,b)=>a+(b||0),0);
            cells.push(cn(nTot+1, r, Number(tot.toFixed(6))));
            // Fórmula SUM en columna Total
            const startCol = colLetra(1); const endCol = colLetra(nTot);
            cells[cells.length-1] = cf(nTot+1, r, `SUM(${startCol}${r+1}:${endCol}${r+1})`, tot);
            r++;
        };

        // Fila Stock con fórmula en cadena
        const mkFilaStock = () => {
            cells.push(ct(0, r, 'Stock Disponible'));
            stockFin.forEach((v, i) => {
                const nbC  = `${colLetra(i+1)}${r-4+1}`; // NB row
                const enC  = `${colLetra(i+1)}${r-3+1}`; // Entradas row
                // Solo preview, Excel no tiene referencia fácil a filas previas sin saber row exacto
                cells.push(cn(i+1, r, Number(v.toFixed(6))));
            });
            cells.push(cn(nTot+1, r, stockFin[nTot-1]));
            r++;
        };

        const nbRow = r;
        mkFila('Necesidades Brutas', nb);
        mkFila('Entradas Previstas', entradas);
        mkFilaStock();
        mkFila('Necesidades Netas', nnetas.map(v => Math.max(0,v)));
        mkFila('Pedidos Planeados', pedidos);
        const lanzRow = r;
        mkFila('Lanzamiento Ordenes', lanzam);
        r++;

        // Resumen órdenes
        cells.push(ct(0, r++, 'RESUMEN DE ÓRDENES DE LANZAMIENTO'));
        cells.push(ct(0, r, 'Período')); cells.push(ct(1, r, 'Cantidad a lanzar')); r++;
        lanzam.forEach((v, i) => {
            if (v > 0) {
                cells.push(ct(0, r, perLabel(i)));
                cells.push(cn(1, r, Number(v.toFixed(4))));
                r++;
            }
        });
        cells.push(ct(0, r, 'TOTAL LANZADO'));
        cells.push(cf(1, r, `SUM(B${lanzRow+1}:${colLetra(nTot)}${lanzRow+1})`,
            lanzam.reduce((a,b)=>a+b,0)));

        const ws = construirHoja(cells, nTot+2, r+1);
        // Ancho de columnas: label ancho, períodos compactos
        const colW = nTot <= 12 ? 10 : nTot <= 26 ? 8 : 7;
        ws['!cols'] = [34, ...Array(nTot).fill(colW), 12].map(w=>({wch:w}));
        descargarExcel(`MRP_${material.replace(/ /g,'_')}_${nTot}per`, 'MRP', ws);
    }

    // --- Inventarios Excel ---
    function exportarExcelInventarios() {
        const cells = [];
        let r = 0;
        cells.push(ct(0, r++, 'Sistema IA de Planificación - Leonardo Carrasco Ocon'));
        cells.push(ct(0, r++, 'Inventario de Materiales'));
        r++;
        ['Material','Unidad','Stock Inicial','Tamaño Lote','Lead Time (sem)'].forEach((h,c) => cells.push(ct(c, r, h)));
        r++;
        const ds = r;
        inventariosData.forEach((item, i) => {
            cells.push(ct(0, r+i, item.material));
            cells.push(ct(1, r+i, item.und));
            cells.push(cn(2, r+i, item.stock));
            cells.push(ct(3, r+i, item.lote));
            cells.push(cn(4, r+i, item.lt));
        });
        r += inventariosData.length;
        r++;
        // Totales
        const stockStart = `C${ds+1}`; const stockEnd = `C${ds+inventariosData.length}`;
        cells.push(ct(0, r, 'Total Stock'));
        cells.push(cf(2, r, `SUM(${stockStart}:${stockEnd})`, inventariosData.reduce((a,b)=>a+b.stock,0)));
        r++;
        cells.push(ct(0, r, 'Promedio Lead Time'));
        const ltStart = `E${ds+1}`; const ltEnd = `E${ds+inventariosData.length}`;
        cells.push(cf(4, r, `AVERAGE(${ltStart}:${ltEnd})`, inventariosData.reduce((a,b)=>a+b.lt,0)/inventariosData.length));

        const ws = construirHoja(cells, 5, r+1);
        ws['!cols'] = [36,10,14,14,18].map(w=>({wch:w}));
        descargarExcel('Inventario_Materiales', 'Inventarios', ws);
    }

    // --- BOM Excel ---
    function exportarExcelBOM() {
        const cells = [];
        let r = 0;
        cells.push(ct(0, r++, 'Sistema IA de Planificación - Leonardo Carrasco Ocon'));
        cells.push(ct(0, r++, 'Lista de Materiales (BOM)'));
        r++;
        ['Producto/Componente','Nivel','Componente','Cantidad','Unidad'].forEach((h,c) => cells.push(ct(c, r, h)));
        r++;
        const ds = r;
        bomData.forEach((item, i) => {
            cells.push(ct(0, r+i, item.prod));
            cells.push(cn(1, r+i, item.nivel));
            cells.push(ct(2, r+i, item.comp));
            cells.push(cn(3, r+i, item.cant));
            cells.push(ct(4, r+i, item.und));
        });
        r += bomData.length;
        r++;
        // COUNTIF por nivel
        [0,1,2].forEach((nivel, i) => {
            const nivStart = `B${ds+1}`; const nivEnd = `B${ds+bomData.length}`;
            cells.push(ct(0, r+i, `Componentes Nivel ${nivel}`));
            cells.push(cf(1, r+i, `COUNTIF(${nivStart}:${nivEnd},${nivel})`, bomData.filter(b=>b.nivel===nivel).length));
        });

        const ws = construirHoja(cells, 5, r+3);
        ws['!cols'] = [32,10,30,12,10].map(w=>({wch:w}));
        descargarExcel('BOM_Lista_Materiales', 'BOM', ws);
    }

    // --- Órdenes de aprovisionamiento ---
    let _ordenesDatos = [];

    function generarOrdenesAprovisionamiento() {
        // Si hay órdenes MRP acumuladas, mostrarlas
        if (typeof ordenesMRP !== 'undefined' && Object.keys(ordenesMRP).length > 0) {
            renderOrdenesAcumuladas();
            return;
        }
        // Fallback: calcular desde PMP + BOM + Inventarios

        // Usar _pmpDatos si ya fue calculado; sino usar valores por defecto
        let totalMPS = 0;
        if (_pmpDatos && _pmpDatos.cantProd) {
            totalMPS = _pmpDatos.cantProd.reduce((a,b)=>a+b,0);
        } else {
            // Fallback: lote mínimo × 20 lotes como estimado
            const loteMin = parseFloat(document.getElementById('loteMin')?.value) || 14;
            totalMPS = loteMin * 20;
        }

        // Construir relación BOM nivel 1
        const relacionBOM = {};
        bomData.forEach(item => {
            if (item.nivel === 1) {
                if (!relacionBOM[item.prod]) relacionBOM[item.prod] = [];
                relacionBOM[item.prod].push({ componente: item.comp, cantidad: item.cant, und: item.und });
            }
        });

        // Calcular necesidades brutas desde BOM × producción total
        let necesidadesBrutas = {};
        // Recorrer todos los productos nivel 0 que tengan componentes nivel 1
        Object.keys(relacionBOM).forEach(prod => {
            relacionBOM[prod].forEach(comp => {
                const nb = totalMPS * comp.cantidad;
                necesidadesBrutas[comp.componente] = (necesidadesBrutas[comp.componente] || 0) + nb;
            });
        });

        // Si no hay nada en BOM nivel 1, intentar con lo que haya
        if (Object.keys(necesidadesBrutas).length === 0) {
            bomData.forEach(item => {
                if (item.nivel >= 1) {
                    necesidadesBrutas[item.comp] = (necesidadesBrutas[item.comp] || 0) + totalMPS * item.cant;
                }
            });
        }

        let necesidadesNetas = {};
        for (let comp in necesidadesBrutas) {
            let inventario = inventariosData.find(i => i.material.includes(comp))?.stock || 0;
            necesidadesNetas[comp] = Math.max(0, necesidadesBrutas[comp] - inventario);
        }

        let ordenesCompra = {};
        for (let comp in necesidadesNetas) {
            let lote = inventariosData.find(i => i.material.includes(comp))?.lote;
            let necesidad = necesidadesNetas[comp];
            if (lote && lote !== "LFL" && parseFloat(lote) > 0) {
                ordenesCompra[comp] = Math.ceil(necesidad / parseFloat(lote)) * parseFloat(lote);
            } else {
                ordenesCompra[comp] = necesidad;
            }
        }

        _ordenesDatos = [];
        let html = `<h4>📊 Órdenes Generadas Automáticamente desde PMP + BOM + Inventarios</h4>
                    <table><thead><tr><th>Componente</th><th>Necesidad Bruta</th><th>Stock Actual</th><th>Necesidad Neta</th><th>Lote</th><th>Orden de Compra</th></tr></thead><tbody>`;
        for (let comp in necesidadesBrutas) {
            let bruta = necesidadesBrutas[comp];
            let stockActual = inventariosData.find(i => i.material.includes(comp))?.stock || 0;
            let neta = necesidadesNetas[comp];
            let lote = inventariosData.find(i => i.material.includes(comp))?.lote || "LFL";
            let orden = ordenesCompra[comp] || 0;
            html += `<tr><td>${comp}</td><td>${bruta}</td><td>${stockActual}</td><td>${neta}</td><td>${lote}</td><td><strong>${orden}</strong></td></tr>`;
            _ordenesDatos.push([comp, bruta, stockActual, neta, lote, orden]);
        }
        html += `</tbody></table>
                 <p><i class="fas fa-sync-alt"></i> <strong>Automático:</strong> Las órdenes se calculan según PMP × BOM - Inventario</p>`;
        document.getElementById('resultadoOrdenes').innerHTML = html;
    }

    function exportarOrdenesCSV() {
        let tabla = document.querySelector("#resultadoOrdenes table");
        if (!tabla) { alert("Primero genera las órdenes"); return; }
        let csv = [];
        let filas = tabla.querySelectorAll("tr");
        for (let fila of filas) {
            let celdas = fila.querySelectorAll("th, td");
            let filaCsv = Array.from(celdas).map(c => `"${c.innerText}"`).join(",");
            csv.push(filaCsv);
        }
        let blob = new Blob([csv.join("\n")], { type: "text/csv" });
        let link = document.createElement("a");
        link.href = URL.createObjectURL(blob);
        link.download = "ordenes_aprovisionamiento.csv";
        link.click();
    }

    function exportarExcelOrdenes() {
        if (!_ordenesDatos.length) { alert("Primero genera las órdenes"); return; }
        const cells = [];
        let r = 0;
        cells.push(ct(0, r++, 'Sistema IA de Planificación - Leonardo Carrasco Ocon'));
        cells.push(ct(0, r++, 'Órdenes de Aprovisionamiento'));
        r++;
        ['Componente','Necesidad Bruta','Stock Actual','Necesidad Neta','Tamaño Lote','Orden de Compra'].forEach((h,c) => cells.push(ct(c, r, h)));
        r++;
        const ds = r;
        _ordenesDatos.forEach((row, i) => {
            cells.push(ct(0, r+i, row[0]));
            cells.push(cn(1, r+i, row[1]));
            cells.push(cn(2, r+i, row[2]));
            // Necesidad Neta = MAX(0, Bruta - Stock)
            const bruCell = `B${ds+i+1}`; const stCell = `C${ds+i+1}`;
            cells.push(cf(3, r+i, `MAX(0,${bruCell}-${stCell})`, row[3]));
            cells.push(ct(4, r+i, String(row[4])));
            cells.push(cn(5, r+i, row[5]));
        });
        r += _ordenesDatos.length;
        r++;
        // Totales
        const bStart = `B${ds+1}`; const bEnd = `B${ds+_ordenesDatos.length}`;
        const nStart = `D${ds+1}`; const nEnd = `D${ds+_ordenesDatos.length}`;
        const oStart = `F${ds+1}`; const oEnd = `F${ds+_ordenesDatos.length}`;
        cells.push(ct(0, r, 'TOTALES'));
        cells.push(cf(1, r, `SUM(${bStart}:${bEnd})`, _ordenesDatos.reduce((a,b)=>a+b[1],0)));
        cells.push(ct(2, r, ''));
        cells.push(cf(3, r, `SUM(${nStart}:${nEnd})`, _ordenesDatos.reduce((a,b)=>a+b[3],0)));
        cells.push(ct(4, r, ''));
        cells.push(cf(5, r, `SUM(${oStart}:${oEnd})`, _ordenesDatos.reduce((a,b)=>a+b[5],0)));

        const ws = construirHoja(cells, 6, r+1);
        ws['!cols'] = [32,16,14,16,14,16].map(w=>({wch:w}));
        descargarExcel('Ordenes_Aprovisionamiento', 'Órdenes', ws);
    }

    async function exportarPDF() {
        const element = document.getElementById('reportContainer');
        const canvas = await html2canvas(element, { scale: 2, backgroundColor: '#0a0e12' });
        const imgData = canvas.toDataURL('image/png');
        const { jsPDF } = window.jspdf;
        const pdf = new jsPDF('p', 'mm', 'a4');
        const imgWidth = 210;
        const pageHeight = 297;
        const imgHeight = (canvas.height * imgWidth) / canvas.width;
        let position = 0;
        pdf.addImage(imgData, 'PNG', 0, position, imgWidth, imgHeight);
        if(imgHeight > pageHeight){
            let heightLeft = imgHeight - pageHeight;
            while(heightLeft > 0){
                position = heightLeft - imgHeight;
                pdf.addPage();
                pdf.addImage(imgData, 'PNG', 0, position, imgWidth, imgHeight);
                heightLeft -= pageHeight;
            }
        }
        pdf.save('Planificacion_Leonardo_Carrasco.pdf');
    }

    // ===============================================================
    // MRP II — CRP, CONTROL PLANTA, COMPRAS, FINANCIERO
    // ===============================================================

    // ── TAB 10: CRP ────────────────────────────────────────────────
    function calcularCRP() {
        const centros  = document.getElementById('crpCentros').value.split(',').map(s=>s.trim()).filter(Boolean);
        const capDisp  = document.getElementById('crpCapDisp').value.split(',').map(Number);
        const hhCentro = document.getElementById('crpHhCentro').value.split(',').map(Number);
        const efic     = document.getElementById('crpEfic').value.split(',').map(Number);
        const semanas  = parseInt(document.getElementById('crpSemanas').value) || 4;
        const prodSem  = document.getElementById('crpProdSem').value.split(',').map(Number);

        if (!centros.length) { alert('⚠️ Ingresa los centros de trabajo'); return; }
        if ([capDisp,hhCentro,efic].some(arr=>arr.some(isNaN))) { alert('⚠️ Revisa los datos numéricos'); return; }

        const th = t => `<th style="background:#10323e;color:#a5f3fc;padding:4px 8px">${t}</th>`;
        const td = (v,color='') => `<td style="padding:3px 7px;text-align:right;${color?'color:'+color+';font-weight:bold':''}">${v}</td>`;
        const tl = t => `<td style="padding:3px 7px">${t}</td>`;

        let semLabels = Array.from({length:semanas},(_,i)=>`S${i+1}`);
        let html2 = `<div style="overflow-x:auto"><table style="width:100%;border-collapse:collapse;font-size:0.78rem">
        <thead><tr>${th('Centro')}${th('Cap.Disp(h)')}${th('HH/par')}${th('Efic.%')}
        ${semLabels.map(s=>th(`Req ${s}(h)`)).join('')}${semLabels.map(s=>th(`Util ${s}%`)).join('')}${th('Estado')}</tr></thead><tbody>`;

        const crpData = [];
        centros.forEach((c,ci) => {
            const capEfec = (capDisp[ci]||0) * ((efic[ci]||100)/100);
            const reqs = prodSem.slice(0,semanas).map(p => p * (hhCentro[ci]||0));
            const utils = reqs.map(r => capEfec > 0 ? (r/capEfec*100) : 0);
            const maxUtil = Math.max(...utils);
            const estado = maxUtil > 100 ? '🔴 Sobrecarga' : maxUtil > 85 ? '🟡 Ajustado' : '🟢 OK';
            const color  = maxUtil > 100 ? '#f87171' : maxUtil > 85 ? '#facc15' : '#4ade80';
            crpData.push({centro:c, capDisp:capDisp[ci], capEfec, hhCentro:hhCentro[ci], efic:efic[ci], reqs, utils, estado, maxUtil});
            html2 += `<tr>${tl(c)}${td((capDisp[ci]||0).toFixed(0))}${td((hhCentro[ci]||0).toFixed(2))}${td((efic[ci]||0).toFixed(0)+'%')}
            ${reqs.map(r=>td(r.toFixed(1))).join('')}
            ${utils.map(u=>td(u.toFixed(1)+'%', u>100?'#f87171':u>85?'#facc15':'')).join('')}
            ${td(estado, color)}</tr>`;
        });
        html2 += `</tbody></table></div>`;

        // Resumen
        const sobrecargados = crpData.filter(c=>c.maxUtil>100);
        const ajustados     = crpData.filter(c=>c.maxUtil>85&&c.maxUtil<=100);
        html2 += `<div style="margin-top:0.8rem;display:flex;gap:1rem;flex-wrap:wrap">
            <div class="ia-insight ${sobrecargados.length?'danger':'success'}" style="flex:1;min-width:200px">
            <i class="fas fa-robot"></i> <strong>IA CRP:</strong>
            ${sobrecargados.length ? `⚠️ ${sobrecargados.map(c=>c.centro).join(', ')} en sobrecarga. Considera tiempo extra o subcontratación.`
            : ajustados.length ? `🟡 ${ajustados.map(c=>c.centro).join(', ')} cerca del límite. Monitorear.`
            : '✅ Todos los centros tienen capacidad suficiente para el plan.'}</div></div>`;

        document.getElementById('resultadoCRP').innerHTML = html2;

        // Gráfico CRP
        if (charts.crp) charts.crp.destroy();
        const ctxCRP = document.getElementById('chartCRP').getContext('2d');
        const bgW = [{ id:'bgW', beforeDraw(c){const x=c.ctx;x.save();x.fillStyle='#ffffff';x.fillRect(0,0,c.width,c.height);x.restore();}}];
        const colores = ['rgba(26,111,168,0.7)','rgba(232,160,32,0.7)','rgba(74,222,128,0.7)','rgba(248,113,113,0.7)','rgba(192,132,252,0.7)'];
        charts.crp = new Chart(ctxCRP, {
            type: 'bar', plugins: bgW,
            data: {
                labels: semLabels,
                datasets: crpData.map((c,i) => ({
                    label: c.centro,
                    data: c.utils,
                    backgroundColor: colores[i % colores.length],
                    borderColor: colores[i % colores.length].replace('0.7','1'),
                    borderWidth: 1
                })).concat([{
                    label: 'Límite 100%',
                    data: Array(semanas).fill(100),
                    type: 'line',
                    borderColor: '#f87171',
                    borderDash: [6,4],
                    borderWidth: 2,
                    pointRadius: 0,
                    backgroundColor: 'transparent'
                }])
            },
            options: {
                responsive: true,
                plugins: {
                    legend:{labels:{color:'#333'}},
                    title:{display:true,text:'CRP — Utilización de Capacidad por Centro (%)',color:'#333',font:{size:13,weight:'bold'}}
                },
                scales: {
                    x:{ticks:{color:'#333'},grid:{color:'#eee'}},
                    y:{ticks:{color:'#333',callback:v=>v+'%'},max:130,title:{display:true,text:'Utilización %',color:'#555'},grid:{color:'#eee'}}
                }
            }
        });
    }

    // ── TAB 11: CONTROL DE PLANTA ──────────────────────────────────
    function calcularSFC() {
        const planif     = document.getElementById('sfcPlanif').value.split(',').map(Number);
        const real       = document.getElementById('sfcReal').value.split(',').map(Number);
        const hPlan      = document.getElementById('sfcHPlan').value.split(',').map(Number);
        const hReal      = document.getElementById('sfcHReal').value.split(',').map(Number);
        const costoPlan  = document.getElementById('sfcCostoPlan').value.split(',').map(Number);
        const costoReal  = document.getElementById('sfcCostoReal').value.split(',').map(Number);

        if (!planif.length||planif.some(isNaN)) { alert('⚠️ Ingresa la producción planificada'); return; }
        const n = planif.length;
        const semanas = Array.from({length:n},(_,i)=>`S${i+1}`);

        const eficProd  = planif.map((p,i) => real[i] && p ? (real[i]/p*100) : 0);
        const eficHoras = hPlan.map((h,i) => hReal[i] && h ? (hReal[i]/h*100) : 0);
        const varCosto  = costoPlan.map((c,i) => costoReal[i] ? costoReal[i]-c : 0);
        const prodAcum  = real.reduce((a,b)=>a+b,0);
        const planAcum  = planif.reduce((a,b)=>a+b,0);
        const eficGlobal= planAcum ? (prodAcum/planAcum*100) : 0;

        const th = t => `<th style="background:#10323e;color:#a5f3fc;padding:4px 8px">${t}</th>`;
        const td = (v,c='') => `<td style="padding:3px 7px;text-align:right;${c?'color:'+c+';font-weight:bold':''}">${v}</td>`;
        const tl = t => `<td style="padding:3px 7px">${t}</td>`;
        const fmtC = v => `S/ ${v.toFixed(2)}`;

        const filas = [
            ['Producción planificada (pares)', planif, v=>v.toFixed(0)],
            ['Producción real (pares)',         real,   v=>v.toFixed(0)],
            ['Eficiencia producción (%)',       eficProd, v=>v.toFixed(1)+'%'],
            ['Horas planificadas',              hPlan,  v=>v.toFixed(0)],
            ['Horas reales',                    hReal,  v=>v.toFixed(0)],
            ['Eficiencia horas (%)',            eficHoras, v=>v.toFixed(1)+'%'],
            ['Costo planificado (S/.)',          costoPlan, fmtC],
            ['Costo real (S/.)',                 costoReal, fmtC],
            ['Variación costo (S/.)',            varCosto, v=>`${v>=0?'+':''}${fmtC(v)}`],
        ].map(([label, arr, fmt]) =>
            `<tr>${tl(label)}${arr.map((v,i) => {
                const isEfic = label.includes('Efic');
                const isVar  = label.includes('Vari');
                const color  = isEfic ? (v<85?'#f87171':v>100?'#4ade80':'') : isVar ? (v>0?'#f87171':'#4ade80') : '';
                return td(fmt(v), color);
            }).join('')}${td(fmt(arr.reduce((a,b)=>a+(typeof b==='number'?b:0),0)))}</tr>`
        ).join('');

        const html2 = `
        <div style="display:flex;gap:1rem;flex-wrap:wrap;margin-bottom:0.8rem">
            <div style="background:#0e2a33;border-radius:0.8rem;padding:0.8rem 1.2rem;text-align:center;min-width:140px">
                <div style="font-size:0.72rem;color:#8bb3cc">Eficiencia Global</div>
                <div style="font-size:1.8rem;font-weight:700;color:${eficGlobal>=85?'#4ade80':'#f87171'}">${eficGlobal.toFixed(1)}%</div>
            </div>
            <div style="background:#0e2a33;border-radius:0.8rem;padding:0.8rem 1.2rem;text-align:center;min-width:140px">
                <div style="font-size:0.72rem;color:#8bb3cc">Prod. Real Total</div>
                <div style="font-size:1.8rem;font-weight:700;color:#00f2fe">${prodAcum.toFixed(0)}</div>
                <div style="font-size:0.65rem;color:#8bb3cc">de ${planAcum.toFixed(0)} planificados</div>
            </div>
            <div style="background:#0e2a33;border-radius:0.8rem;padding:0.8rem 1.2rem;text-align:center;min-width:140px">
                <div style="font-size:0.72rem;color:#8bb3cc">Variación Costo Total</div>
                <div style="font-size:1.8rem;font-weight:700;color:${varCosto.reduce((a,b)=>a+b,0)>0?'#f87171':'#4ade80'}">
                    ${varCosto.reduce((a,b)=>a+b,0)>=0?'+':''}S/ ${varCosto.reduce((a,b)=>a+b,0).toFixed(2)}</div>
            </div>
        </div>
        <div style="overflow-x:auto"><table style="width:100%;border-collapse:collapse;font-size:0.78rem">
        <thead><tr>${th('Concepto')}${semanas.map(th).join('')}${th('Total')}</tr></thead>
        <tbody>${filas}</tbody></table></div>
        <div class="ia-insight ${eficGlobal>=85?'success':'danger'}" style="margin-top:0.8rem">
        <i class="fas fa-robot"></i> <strong>IA Control Planta:</strong>
        ${eficGlobal>=95?'✅ Excelente eficiencia. La planta opera cerca de su óptimo.':
          eficGlobal>=85?'📈 Eficiencia aceptable. Revisar cuellos de botella para mejorar.':
          '⚠️ Eficiencia baja. Identificar causas: paradas, reprocesos, falta de material.'}</div>`;

        document.getElementById('resultadoSFC').innerHTML = html2;

        // Gráfico SFC
        if (charts.sfc) charts.sfc.destroy();
        const ctxSFC = document.getElementById('chartSFC').getContext('2d');
        const bgW = [{ id:'bgW', beforeDraw(c){const x=c.ctx;x.save();x.fillStyle='#ffffff';x.fillRect(0,0,c.width,c.height);x.restore();}}];
        charts.sfc = new Chart(ctxSFC, {
            type: 'bar', plugins: bgW,
            data: {
                labels: semanas,
                datasets: [
                    {label:'Planificado (pares)', data:planif, backgroundColor:'rgba(26,111,168,0.6)', borderColor:'#1A6FA8', borderWidth:1},
                    {label:'Real (pares)',         data:real,   backgroundColor:'rgba(74,222,128,0.6)', borderColor:'#4ade80', borderWidth:1},
                    {label:'Eficiencia %',         data:eficProd, type:'line', borderColor:'#E8A020', borderWidth:2,
                     pointBackgroundColor:'#E8A020', yAxisID:'y2', tension:0.3}
                ]
            },
            options: {
                responsive:true,
                plugins:{legend:{labels:{color:'#333'}}, title:{display:true,text:'Control de Planta — Real vs Planificado',color:'#333',font:{size:13,weight:'bold'}}},
                scales:{
                    x:{ticks:{color:'#333'},grid:{color:'#eee'}},
                    y:{position:'left',ticks:{color:'#1A6FA8'},title:{display:true,text:'Pares',color:'#1A6FA8'},grid:{color:'#eee'}},
                    y2:{position:'right',ticks:{color:'#E8A020',callback:v=>v+'%'},title:{display:true,text:'Eficiencia %',color:'#E8A020'},grid:{drawOnChartArea:false}}
                }
            }
        });
    }

    // ── TAB 12: COMPRAS ────────────────────────────────────────────
    let comprasData = [];

    function generarComprasDesdeOrdenes() {
        comprasData = [];
        // Leer órdenes del MRP si existen
        if (_mrpDatos && _mrpDatos.lanzam) {
            const { lanzam, material, lote } = _mrpDatos;
            const inv = inventariosData.find(i => i.material === material);
            const precio = 0; // el usuario lo llena
            lanzam.forEach((v, i) => {
                if (v > 0) {
                    const hoy = new Date();
                    const fechaPedido = new Date(hoy.getTime() + i*7*24*3600*1000);
                    const lt = inv ? inv.lt : 0;
                    const fechaEntrega = new Date(fechaPedido.getTime() + lt*7*24*3600*1000);
                    comprasData.push({
                        material, proveedor:'', cantidad:v,
                        precioUnit:0, total:0,
                        fechaPedido: fechaPedido.toISOString().split('T')[0],
                        fechaEntrega: fechaEntrega.toISOString().split('T')[0],
                        estado:'Pendiente'
                    });
                }
            });
        }
        // Agregar materiales del inventario que tengan lote definido
        inventariosData.forEach(inv => {
            if (inv.stock < 50 && inv.lote !== 'LFL') {
                comprasData.push({
                    material:inv.material, proveedor:'', cantidad:parseFloat(inv.lote)||0,
                    precioUnit:0, total:0,
                    fechaPedido: new Date().toISOString().split('T')[0],
                    fechaEntrega:'', estado:'Por evaluar'
                });
            }
        });
        renderTablaCompras();
    }

    function agregarFilaCompra() {
        comprasData.push({ material:'', proveedor:'', cantidad:0, precioUnit:0, total:0,
                           fechaPedido:new Date().toISOString().split('T')[0], fechaEntrega:'', estado:'Pendiente' });
        renderTablaCompras();
    }

    function renderTablaCompras() {
        const tbody = document.getElementById('tbodyCompras');
        if (!tbody) return;
        const estadoColor = {'Pendiente':'#facc15','Confirmado':'#4ade80','Recibido':'#00f2fe','Por evaluar':'#c084fc','Cancelado':'#f87171'};
        tbody.innerHTML = comprasData.map((c,i) => `
            <tr>
                <td><input type="text" value="${c.material}" oninput="comprasData[${i}].material=this.value" style="width:150px"></td>
                <td><input type="text" value="${c.proveedor}" oninput="comprasData[${i}].proveedor=this.value" style="width:120px" placeholder="Proveedor"></td>
                <td><input type="number" value="${c.cantidad}" oninput="comprasData[${i}].cantidad=parseFloat(this.value)||0;actualizarTotalCompra(${i})" style="width:80px"></td>
                <td><input type="number" value="${c.precioUnit}" oninput="comprasData[${i}].precioUnit=parseFloat(this.value)||0;actualizarTotalCompra(${i})" style="width:80px" placeholder="0.00"></td>
                <td id="totalCompra_${i}" style="text-align:right;padding:3px 6px">S/ ${(c.cantidad*c.precioUnit).toFixed(2)}</td>
                <td><input type="date" value="${c.fechaPedido}" oninput="comprasData[${i}].fechaPedido=this.value" style="width:130px"></td>
                <td><input type="date" value="${c.fechaEntrega}" oninput="comprasData[${i}].fechaEntrega=this.value" style="width:130px"></td>
                <td><select oninput="comprasData[${i}].estado=this.value" style="width:120px;color:${estadoColor[c.estado]||'#fff'}">
                    ${['Pendiente','Confirmado','Recibido','Por evaluar','Cancelado'].map(e=>`<option value="${e}" ${c.estado===e?'selected':''}>${e}</option>`).join('')}
                </select></td>
            </tr>`).join('');
        // Total general
        const totalG = comprasData.reduce((a,c)=>a+c.cantidad*c.precioUnit,0);
        document.getElementById('tblCompras').querySelector('tfoot')?.remove();
        const tfoot = document.createElement('tfoot');
        tfoot.innerHTML = `<tr style="background:#0e2a33;font-weight:bold">
            <td colspan="4" style="padding:4px 7px">TOTAL COMPRAS</td>
            <td style="padding:4px 7px;text-align:right;color:#00f2fe">S/ ${totalG.toFixed(2)}</td>
            <td colspan="3"></td></tr>`;
        document.getElementById('tblCompras').appendChild(tfoot);
    }

    function actualizarTotalCompra(i) {
        const el = document.getElementById(`totalCompra_${i}`);
        if (el) el.textContent = `S/ ${(comprasData[i].cantidad*comprasData[i].precioUnit).toFixed(2)}`;
        renderTablaCompras();
    }

    // ── TAB 13: FINANCIERO ─────────────────────────────────────────
    function calcularFinanciero() {
        const precioVenta  = parseFloat(document.getElementById('finPrecioVenta').value);
        const costoMP      = parseFloat(document.getElementById('finCostoMP').value);
        const costoMO      = parseFloat(document.getElementById('finCostoMO').value);
        const cif          = parseFloat(document.getElementById('finCIF').value);
        const gastosAdmin  = parseFloat(document.getElementById('finGastosAdmin').value);
        const gastosVentas = parseFloat(document.getElementById('finGastosVentas').value);

        if ([precioVenta,costoMP,costoMO,cif,gastosAdmin,gastosVentas].some(isNaN)) {
            alert('⚠️ Completa todos los campos financieros'); return;
        }

        // Tomar producción del PAP o PMP si existen
        let prodMensual = [];
        let demMensual  = [];
        if (_papDatos && _papDatos.demandas) {
            demMensual  = _papDatos.demandas;
            prodMensual = _papDatos.reqP || _papDatos.demandas;
        } else if (_pmpDatos && _pmpDatos.cantProd) {
            const total = _pmpDatos.cantProd.reduce((a,b)=>a+b,0);
            prodMensual = Array(12).fill(total/12);
            demMensual  = prodMensual;
        } else {
            alert('⚠️ Primero calcula el PAP o PMP para obtener la producción mensual'); return;
        }

        const n = Math.min(prodMensual.length, 12);
        const meses = ['Ene','Feb','Mar','Abr','May','Jun','Jul','Ago','Sep','Oct','Nov','Dic'].slice(0,n);

        const costoUnitario = costoMP + costoMO + cif;
        const margenUnit    = precioVenta - costoUnitario;

        const ingresos   = demMensual.slice(0,n).map(d => d * precioVenta);
        const costoMPs   = prodMensual.slice(0,n).map(p => p * costoMP);
        const costoMOs   = prodMensual.slice(0,n).map(p => p * costoMO);
        const cifs       = prodMensual.slice(0,n).map(p => p * cif);
        const costoProd  = prodMensual.slice(0,n).map(p => p * costoUnitario);
        const utilBruta  = ingresos.map((ing,i) => ing - costoProd[i]);
        const gastosOp   = Array(n).fill(gastosAdmin + gastosVentas);
        const utilNeta   = utilBruta.map((u,i) => u - gastosOp[i]);
        const margenPct  = ingresos.map((ing,i) => ing>0 ? (utilNeta[i]/ing*100) : 0);

        const fmtC = v => `S/ ${v.toLocaleString('es-PE',{minimumFractionDigits:2,maximumFractionDigits:2})}`;
        const th = t => `<th style="background:#10323e;color:#a5f3fc;padding:4px 6px;font-size:0.72rem">${t}</th>`;
        const td = (v,c='') => `<td style="padding:3px 6px;text-align:right;font-size:0.75rem;${c?'color:'+c+';font-weight:bold':''}">${v}</td>`;
        const tl = t => `<td style="padding:3px 6px;font-size:0.75rem">${t}</td>`;

        const tot = arr => arr.reduce((a,b)=>a+b,0);
        const mkFila = (label, arr, fmt, color='') =>
            `<tr>${tl(label)}${arr.map(v=>td(fmt(v),color)).join('')}${td(fmt(tot(arr)),color)}</tr>`;

        const utilTot    = tot(utilNeta);
        const ingresoTot = tot(ingresos);
        const margenG    = ingresoTot>0 ? utilTot/ingresoTot*100 : 0;

        // KPIs
        const html2 = `
        <div style="display:flex;gap:1rem;flex-wrap:wrap;margin-bottom:1rem">
            ${[
                ['Ingresos Totales', fmtC(ingresoTot), '#00f2fe'],
                ['Costo Total Prod.', fmtC(tot(costoProd)), '#facc15'],
                ['Utilidad Neta Total', fmtC(utilTot), utilTot>=0?'#4ade80':'#f87171'],
                ['Margen Neto Global', margenG.toFixed(2)+'%', margenG>=15?'#4ade80':margenG>=5?'#facc15':'#f87171'],
                ['Costo Unit. Prod.', fmtC(costoUnitario), '#c084fc'],
                ['Margen por par', fmtC(margenUnit), margenUnit>0?'#4ade80':'#f87171'],
            ].map(([label,val,color])=>`
            <div style="background:#0e2a33;border-radius:0.8rem;padding:0.8rem 1.2rem;text-align:center;min-width:150px;flex:1">
                <div style="font-size:0.72rem;color:#8bb3cc;margin-bottom:4px">${label}</div>
                <div style="font-size:1.3rem;font-weight:700;color:${color}">${val}</div>
            </div>`).join('')}
        </div>
        <div style="overflow-x:auto"><table style="width:100%;border-collapse:collapse">
        <thead><tr>${th('Concepto')}${meses.map(th).join('')}${th('TOTAL')}</tr></thead>
        <tbody>
        ${mkFila('Producción (pares)', prodMensual.slice(0,n), v=>v.toFixed(1))}
        ${mkFila('Ingresos (S/.)', ingresos, fmtC, '#00f2fe')}
        ${mkFila('Costo MP (S/.)', costoMPs, fmtC)}
        ${mkFila('Costo MO (S/.)', costoMOs, fmtC)}
        ${mkFila('CIF (S/.)', cifs, fmtC)}
        ${mkFila('Costo Producción (S/.)', costoProd, fmtC)}
        ${mkFila('Utilidad Bruta (S/.)', utilBruta, fmtC, '#facc15')}
        ${mkFila('Gastos Operativos (S/.)', gastosOp, fmtC)}
        ${mkFila('Utilidad Neta (S/.)', utilNeta, fmtC, utilTot>=0?'#4ade80':'#f87171')}
        ${mkFila('Margen Neto (%)', margenPct, v=>v.toFixed(2)+'%')}
        </tbody></table></div>
        <div class="ia-insight ${margenG>=15?'success':margenG>=5?'':'danger'}" style="margin-top:0.8rem">
        <i class="fas fa-robot"></i> <strong>IA Financiero:</strong>
        ${margenG>=20?'✅ Excelente margen. El negocio es muy rentable.':
          margenG>=10?'📈 Margen aceptable. Hay espacio para mejorar costos.':
          margenG>=0?'⚠️ Margen bajo. Revisar estructura de costos o precio de venta.':
          '🔴 Negocio en pérdida. Acción urgente requerida.'}</div>`;

        document.getElementById('resultadoFinanciero').innerHTML = html2;

        // Gráfico financiero
        if (charts.fin) charts.fin.destroy();
        const ctxFin = document.getElementById('chartFinanciero').getContext('2d');
        const bgW = [{ id:'bgW', beforeDraw(c){const x=c.ctx;x.save();x.fillStyle='#ffffff';x.fillRect(0,0,c.width,c.height);x.restore();}}];
        charts.fin = new Chart(ctxFin, {
            type:'bar', plugins:bgW,
            data:{
                labels:meses,
                datasets:[
                    {label:'Ingresos (S/.)',       data:ingresos,  backgroundColor:'rgba(26,111,168,0.7)',  yAxisID:'y'},
                    {label:'Costo Producción (S/.)',data:costoProd, backgroundColor:'rgba(248,113,113,0.7)',yAxisID:'y'},
                    {label:'Utilidad Neta (S/.)',   data:utilNeta,  backgroundColor:'rgba(74,222,128,0.7)', yAxisID:'y'},
                    {label:'Margen Neto (%)',       data:margenPct, type:'line', borderColor:'#E8A020',
                     borderWidth:2, pointBackgroundColor:'#E8A020', yAxisID:'y2', tension:0.3}
                ]
            },
            options:{
                responsive:true,
                plugins:{legend:{labels:{color:'#333'}},
                         title:{display:true,text:'Plan Financiero — Ingresos, Costos y Utilidad Mensual',color:'#333',font:{size:13,weight:'bold'}}},
                scales:{
                    x:{ticks:{color:'#333'},grid:{color:'#eee'}},
                    y:{position:'left',ticks:{color:'#333',callback:v=>'S/.'+v.toLocaleString()},title:{display:true,text:'S/.',color:'#555'},grid:{color:'#eee'}},
                    y2:{position:'right',ticks:{color:'#E8A020',callback:v=>v.toFixed(1)+'%'},title:{display:true,text:'Margen %',color:'#E8A020'},grid:{drawOnChartArea:false}}
                }
            }
        });
    }

    // ===============================================================
    // ERP, RESPALDO Y PORTADA
    // ===============================================================

    function actualizarERP() {
        const now = new Date();
        const el = document.getElementById('erpFechaHora');
        if (el) el.textContent = now.toLocaleString('es-PE');

        const status = document.getElementById('erpStatus');

        // ── MD04: MRP ────────────────────────────────────────────────
        const md04 = document.getElementById('erpMD04');
        if (md04 && _mrpDatos) {
            const { nb, stockFin, lanzam, material, lote, lt, nTot } = _mrpDatos;
            const perLabel = i => i < _mrpDatos.nPrev
                ? `S-${_mrpDatos.nPrev-i}` : `S${i-_mrpDatos.nPrev+1}`;
            const mkRow = (bg, label, arr) =>
                `<tr style="background:${bg}">
                    <td style="padding:2px 5px;font-weight:600;font-size:0.7rem">${label}</td>
                    ${arr.map(v=>`<td style="padding:2px 5px;text-align:right;font-size:0.7rem">${typeof v==='number'?v.toFixed(2):v}</td>`).join('')}
                </tr>`;
            const headers = Array.from({length:nTot},(_,i)=>perLabel(i));
            md04.innerHTML = `
                <div style="font-size:0.68rem;color:#0a3055;margin-bottom:4px">
                    Material: <strong>${material}</strong> | Lote: <strong>${lote}</strong> | LT: <strong>${lt}</strong>
                </div>
                <div style="overflow-x:auto"><table style="width:100%;border-collapse:collapse;font-size:0.7rem">
                <thead><tr style="background:#d0e4f0">
                    <th style="padding:2px 5px;text-align:left">Concepto</th>
                    ${headers.map(h=>`<th style="padding:2px 5px;text-align:right">${h}</th>`).join('')}
                </tr></thead><tbody>
                ${mkRow('#fff','Nec. Brutas', nb)}
                ${mkRow('#f0f8ff','Stock Disp.', stockFin)}
                ${mkRow('#e8f5e9','🚀 Lanzamiento', lanzam)}
                </tbody></table></div>`;
        } else if (md04) {
            md04.innerHTML = '<div style="color:#888;font-size:0.72rem">Ejecuta el MRP (Tab ⚙️) para ver datos</div>';
        }

        // ── MC87: PAP ────────────────────────────────────────────────
        const mc87 = document.getElementById('erpMC87');
        if (mc87 && _papDatos) {
            const { demandas, meses, p1, p2, p3, p4 } = _papDatos;
            const planes = [p1.CT, p2.CT, p3.CT, p4.CT];
            const mejor  = planes.indexOf(Math.min(...planes)) + 1;
            const fmtC   = v => 'S/. ' + v.toLocaleString('es-PE',{minimumFractionDigits:2,maximumFractionDigits:2});
            mc87.innerHTML = `
                <div style="font-size:0.7rem;margin-bottom:6px">
                    <span style="background:#0a3055;color:white;padding:2px 8px;border-radius:3px">Plan óptimo: Plan ${mejor}</span>
                    <span style="color:#0a3055;font-weight:700;margin-left:8px">Costo: ${fmtC(planes[mejor-1])}</span>
                </div>
                <table style="width:100%;border-collapse:collapse;font-size:0.7rem">
                <thead><tr style="background:#d0e4f0">
                    <th style="padding:2px 5px;text-align:left">Plan</th>
                    <th style="padding:2px 5px;text-align:right">Costo Total</th>
                    <th style="padding:2px 5px;text-align:right">S/./par</th>
                    <th style="padding:2px 5px;text-align:center">Estado</th>
                </tr></thead><tbody>
                ${['Persecución','Nivelación','Subcontrat.','T.Extra'].map((nom,i)=>`
                    <tr style="background:${i===mejor-1?'#e8f5e9':'#fff'}">
                        <td style="padding:2px 5px">Plan ${i+1} — ${nom}</td>
                        <td style="padding:2px 5px;text-align:right">${fmtC(planes[i])}</td>
                        <td style="padding:2px 5px;text-align:right">${fmtC(planes[i]/_papDatos.params.totalReq)}</td>
                        <td style="padding:2px 5px;text-align:center">${i===mejor-1?'✅ SELECCIONADO':''}</td>
                    </tr>`).join('')}
                </tbody></table>`;
        } else if (mc87) {
            mc87.innerHTML = '<div style="color:#888;font-size:0.72rem">Ejecuta el PAP (Tab 🏭) para ver datos</div>';
        }

        // ── CS03: BOM ────────────────────────────────────────────────
        const cs03 = document.getElementById('erpCS03');
        if (cs03) {
            const nivelColor = ['#0a3055','#1a6fa8','#2aa3b3','#4ade80'];
            cs03.innerHTML = `<table style="width:100%;border-collapse:collapse;font-size:0.7rem">
            <thead><tr style="background:#d0e4f0">
                <th style="padding:2px 5px;text-align:left">Nivel</th>
                <th style="padding:2px 5px;text-align:left">Componente</th>
                <th style="padding:2px 5px;text-align:right">Cant.</th>
                <th style="padding:2px 5px;text-align:left">Und.</th>
            </tr></thead><tbody>
            ${bomData.map(item=>`
                <tr style="background:#fff">
                    <td style="padding:2px 5px">
                        <span style="background:${nivelColor[item.nivel]||'#555'};color:white;padding:1px 5px;border-radius:3px;font-size:0.65rem">N${item.nivel}</span>
                    </td>
                    <td style="padding:2px 5px;padding-left:${item.nivel*12+5}px">${item.comp}</td>
                    <td style="padding:2px 5px;text-align:right">${item.cant}</td>
                    <td style="padding:2px 5px">${item.und}</td>
                </tr>`).join('')}
            </tbody></table>`;
        }

        // ── MMBE: Inventario ─────────────────────────────────────────
        const mmbe = document.getElementById('erpMMBE');
        if (mmbe) {
            sincronizarInventarios();
            mmbe.innerHTML = `<table style="width:100%;border-collapse:collapse;font-size:0.7rem">
            <thead><tr style="background:#d0e4f0">
                <th style="padding:2px 5px;text-align:left">Material</th>
                <th style="padding:2px 5px;text-align:right">Stock</th>
                <th style="padding:2px 5px;text-align:left">Und</th>
                <th style="padding:2px 5px;text-align:left">Lote</th>
                <th style="padding:2px 5px;text-align:right">LT</th>
                <th style="padding:2px 5px;text-align:center">Estado</th>
            </tr></thead><tbody>
            ${inventariosData.map(inv=>{
                const estado = inv.stock === 0 ? '🔴 Sin stock' : inv.stock < 50 ? '🟡 Bajo' : '🟢 OK';
                return `<tr style="background:#fff">
                    <td style="padding:2px 5px;font-size:0.65rem">${inv.material}</td>
                    <td style="padding:2px 5px;text-align:right;font-weight:700">${inv.stock}</td>
                    <td style="padding:2px 5px">${inv.und}</td>
                    <td style="padding:2px 5px">${inv.lote}</td>
                    <td style="padding:2px 5px;text-align:right">${inv.lt}</td>
                    <td style="padding:2px 5px;text-align:center;font-size:0.65rem">${estado}</td>
                </tr>`;
            }).join('')}
            </tbody></table>`;
        }

        // ── CM01: CRP ────────────────────────────────────────────────
        const cm01 = document.getElementById('erpCM01');
        if (cm01) {
            const crpDiv = document.getElementById('resultadoCRP');
            if (crpDiv && crpDiv.querySelector('table')) {
                cm01.innerHTML = '<div style="font-size:0.7rem;color:#0a3055">Ver Tab ⚡ CRP para detalle completo</div>' +
                    '<div style="font-size:0.68rem;color:#555;margin-top:4px">✅ CRP calculado — datos disponibles</div>';
            } else {
                cm01.innerHTML = '<div style="color:#888;font-size:0.72rem">Ejecuta el CRP (Tab ⚡) para ver datos</div>';
            }
        }

        // ── ME2M: Compras ────────────────────────────────────────────
        const me2m = document.getElementById('erpME2M');
        if (me2m) {
            if (comprasData.length > 0) {
                const total = comprasData.reduce((a,c)=>a+c.cantidad*c.precioUnit,0);
                me2m.innerHTML = `
                <table style="width:100%;border-collapse:collapse;font-size:0.7rem">
                <thead><tr style="background:#d0e4f0">
                    <th style="padding:2px 5px;text-align:left">Material</th>
                    <th style="padding:2px 5px;text-align:right">Cant.</th>
                    <th style="padding:2px 5px;text-align:right">Total S/.</th>
                    <th style="padding:2px 5px;text-align:left">Estado</th>
                </tr></thead><tbody>
                ${comprasData.map(c=>`
                    <tr style="background:#fff">
                        <td style="padding:2px 5px;font-size:0.65rem">${c.material}</td>
                        <td style="padding:2px 5px;text-align:right">${c.cantidad.toFixed(2)}</td>
                        <td style="padding:2px 5px;text-align:right">${(c.cantidad*c.precioUnit).toFixed(2)}</td>
                        <td style="padding:2px 5px;font-size:0.65rem">${c.estado}</td>
                    </tr>`).join('')}
                <tr style="background:#e8f5e9;font-weight:700">
                    <td colspan="2" style="padding:2px 5px">TOTAL</td>
                    <td style="padding:2px 5px;text-align:right">S/. ${total.toFixed(2)}</td>
                    <td></td>
                </tr></tbody></table>`;
            } else {
                me2m.innerHTML = '<div style="color:#888;font-size:0.72rem">Ejecuta Compras (Tab 🛒) para ver órdenes</div>';
            }
        }

        if (status) status.textContent = 'Pantallas actualizadas — ' + now.toLocaleTimeString('es-PE');
    }

    function renderRespaldo() {
        // Glosario
        const terminos = [
            ['MRP','Material Requirements Planning — Planificación de necesidades de materiales'],
            ['MRP II','Manufacturing Resource Planning — Sistema integral que amplía el MRP con capacidad, finanzas y control de planta'],
            ['PAP','Plan Agregado de Producción — Plan de producción a mediano plazo que equilibra demanda y capacidad'],
            ['PMP','Plan Maestro de Producción — Desagrega el PAP por producto y período'],
            ['BOM','Bill of Materials — Lista de materiales que componen un producto'],
            ['CRP','Capacity Requirements Planning — Planificación de requerimientos de capacidad'],
            ['Lead Time (LT)','Tiempo de aprovisionamiento — Tiempo entre emitir la orden y recibirla'],
            ['Necesidades Brutas (NB)','Cantidad total requerida de un material en un período'],
            ['Necesidades Netas (NN)','NB menos el stock disponible — lo que realmente hay que pedir'],
            ['Lanzamiento de Órdenes','Momento en que se emite la orden, adelantado por el Lead Time'],
            ['Stock de Seguridad (SS)','Inventario mínimo para protegerse contra variaciones de demanda'],
            ['LFL (Lot for Lot)','Política de lote: pedir exactamente lo que se necesita cada período'],
            ['Promedio Móvil (PM)','Método de pronóstico que promedia los últimos k períodos'],
            ['Suavizado Exponencial','Pronóstico que da más peso a los datos recientes según alfa (α)'],
            ['EPAM','Error Porcentual Absoluto Medio — mide la precisión del pronóstico'],
            ['DAM','Desviación Absoluta Media — promedio de los errores absolutos'],
            ['ECM','Error Cuadrático Medio — penaliza errores grandes más que el DAM'],
            ['Estrategia Persecución','PAP que varía la fuerza laboral para seguir exactamente la demanda'],
            ['Estrategia Nivelación','PAP que mantiene producción constante, absorbiendo variaciones con inventario'],
            ['CIF','Costos Indirectos de Fabricación — costos que no son MP ni MO directa'],
        ];
        const el = document.getElementById('glosario');
        if (el) el.innerHTML = terminos.map(([t,d])=>`
            <div style="background:#0f1a1f;border:1px solid #2a4b5c;border-radius:0.5rem;padding:0.6rem">
                <div style="font-weight:700;color:#00f2fe;font-size:0.8rem">${t}</div>
                <div style="font-size:0.75rem;color:#8bb3cc;margin-top:2px">${d}</div>
            </div>`).join('');

        // Fórmulas
        const formulas = [
            ['Promedio Móvil', 'F(t+1) = [ D(t) + D(t-1) + ... + D(t-k+1) ] / k'],
            ['Suavizado Exponencial', 'F(t+1) = α × D(t) + (1-α) × F(t)'],
            ['Regresión Lineal', 'ŷ = a + b·x | b = (n·ΣXY − ΣX·ΣY) / (n·ΣX² − (ΣX)²) | a = (ΣY − b·ΣX) / n'],
            ['EPAM', 'EPAM = (1/n) × Σ |e(t)/D(t)| × 100%'],
            ['DAM', 'DAM = Σ |D(t) − F(t)| / n'],
            ['ECM', 'ECM = Σ [D(t) − F(t)]² / n'],
            ['Requerimiento Producción PAP', 'ReqP(t) = D(t) + SS(t) − Inv(t-1)'],
            ['Costo Lineal Plan1', 'CL = Σ [ HorasReq(t) × Costo/hora ]'],
            ['Costo Nivelación', 'CL = promTrab × HDisp × Costo/hora × n_períodos'],
            ['Producción Nivelada', 'ProdNiv = promTrab × HDisp / HH_par'],
            ['Necesidades Netas MRP', 'NN(t) = max(0, NB(t) − StockDisp(t))'],
            ['Stock Disponible MRP', 'StockDisp(t) = StockDisp(t-1) + Entradas(t) − NB(t)'],
            ['Lanzamiento Orden MRP', 'Lanzar en período (t − LT) la cantidad pedida en t'],
            ['Lote EOQ (referencia)', 'Q* = √(2·D·S / H) donde S=costo pedido, H=costo mantenimiento'],
            ['Utilidad Bruta', 'UB = Ingresos − Costo de Producción'],
            ['Utilidad Neta', 'UN = UB − Gastos Operativos (Admin + Ventas)'],
            ['Margen Neto', 'Margen = (UN / Ingresos) × 100%'],
            ['Correlación (r)', 'r = [n·ΣXY − ΣX·ΣY] / √[(n·ΣX²−(ΣX)²)·(n·ΣY²−(ΣY)²)]'],
        ];
        const fel = document.getElementById('formulasRespaldo');
        if (fel) fel.innerHTML = `<div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(340px,1fr));gap:0.5rem">
            ${formulas.map(([nombre,formula])=>`
            <div style="background:#0f1a1f;border:1px solid #2a4b5c;border-left:3px solid #00f2fe;border-radius:0.5rem;padding:0.6rem">
                <div style="font-weight:700;color:#eef2ff;font-size:0.78rem;margin-bottom:3px">${nombre}</div>
                <div style="font-family:monospace;font-size:0.72rem;color:#a5f3fc;background:#0a1419;padding:4px 8px;border-radius:4px">${formula}</div>
            </div>`).join('')}</div>`;

        // Bibliografía
        const biblio = [
            ['Chase, Aquilano & Jacobs (2009)','Administración de Operaciones — Producción y Cadena de Suministros','McGraw-Hill, 12ª Ed.'],
            ['Vollmann, Berry, Whybark & Jacobs (2005)','Manufacturing Planning and Control for Supply Chain Management','McGraw-Hill, 5ª Ed.'],
            ['Chopra & Meindl (2013)','Administración de la Cadena de Suministro','Pearson, 5ª Ed.'],
            ['Sipper & Bulfin (1998)','Planeación y Control de la Producción','McGraw-Hill'],
            ['Orlicky, J. (1975)','Material Requirements Planning','McGraw-Hill — Obra original del MRP'],
            ['Wight, O. (1984)','Manufacturing Resource Planning: MRP II','Oliver Wight Publications — Obra original del MRP II'],
            ['APICS Dictionary (2022)','Terminology in Operations Management','Association for Supply Chain Management'],
            ['Montgomery, D.C. (2013)','Introduction to Statistical Quality Control','Wiley, 7ª Ed.'],
        ];
        const bel = document.getElementById('bibliografiaRespaldo');
        if (bel) bel.innerHTML = `<div style="display:flex;flex-direction:column;gap:0.5rem">
            ${biblio.map(([autor,titulo,editorial],i)=>`
            <div style="background:#0f1a1f;border:1px solid #2a4b5c;border-radius:0.5rem;padding:0.6rem;display:flex;gap:0.8rem;align-items:flex-start">
                <span style="background:#00f2fe;color:#0a0e12;font-weight:700;font-size:0.7rem;padding:2px 7px;border-radius:1rem;min-width:24px;text-align:center">${i+1}</span>
                <div>
                    <div style="font-weight:600;color:#eef2ff;font-size:0.8rem">${titulo}</div>
                    <div style="font-size:0.72rem;color:#8bb3cc">${autor}</div>
                    <div style="font-size:0.7rem;color:#5f8ca3;font-style:italic">${editorial}</div>
                </div>
            </div>`).join('')}</div>`;
    }

    function inicializarPortada() {
        const fechaEl = document.getElementById('portadaFecha');
        if (fechaEl && !fechaEl.value) {
            fechaEl.value = new Date().toLocaleDateString('es-PE',{year:'numeric',month:'long',day:'numeric'});
        }
    }

    // Datos PMP por SKU guardados en memoria
    let pmpSkuData = []; // [{prod, ventas, invIni, ss}]

    function cargarSKUsdesdeBOM() {
        // Obtener TODOS los productos nivel 0 del BOM
        const prods = [...new Set(bomData.filter(b => b.nivel === 0).map(b => b.prod))];
        const grid  = document.getElementById('pmpSkusGrid');
        if (!grid) return;

        // Preservar valores que el usuario ya ingresó
        const prevData = {};
        pmpSkuData.forEach(s => { prevData[s.prod] = s; });

        // Actualizar pmpSkuData con los productos del BOM
        pmpSkuData = prods.map(prod => ({
            prod,
            ventas: prevData[prod]?.ventas || '',
            invIni: prevData[prod]?.invIni || '',
            ss:     prevData[prod]?.ss     || '',
        }));

        // Renderizar grid dinámico
        grid.innerHTML = pmpSkuData.map((sku, i) => `
            <div style="background:#0f1a1f;border:1px solid #2a4b5c;border-radius:0.8rem;padding:0.8rem;margin-bottom:0.5rem">
                <div style="font-weight:700;color:#00f2fe;font-size:0.82rem;margin-bottom:0.5rem">
                    📦 ${sku.prod}
                </div>
                <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:0.5rem">
                    <div>
                        <label style="font-size:0.68rem;color:#8bb3cc;text-transform:uppercase">Ventas prev. (pares)</label>
                        <input type="number" id="pmp_ventas_${i}" value="${sku.ventas}"
                            placeholder="Pares año anterior" oninput="pmpSkuData[${i}].ventas=this.value">
                    </div>
                    <div>
                        <label style="font-size:0.68rem;color:#8bb3cc;text-transform:uppercase">Inv. inicial (pares)</label>
                        <input type="number" id="pmp_invini_${i}" value="${sku.invIni}"
                            placeholder="Stock actual" oninput="pmpSkuData[${i}].invIni=this.value">
                    </div>
                    <div>
                        <label style="font-size:0.68rem;color:#8bb3cc;text-transform:uppercase">Stock seguridad (pares)</label>
                        <input type="number" id="pmp_ss_${i}" value="${sku.ss}"
                            placeholder="SS mínimo" oninput="pmpSkuData[${i}].ss=this.value">
                    </div>
                </div>
            </div>`).join('');

        if (!prods.length) {
            grid.innerHTML = '<p style="color:#f87171;font-size:0.8rem">⚠️ No hay productos nivel 0 en el BOM. Agrégalos primero en la pestaña 🔧 BOM.</p>';
        }
    }

        // ── Órdenes MRP acumuladas ─────────────────────────────────────────────
    let ordenesMRP = {}; // { material: { lanzam, nb, lote, lt, modo, nPrev, nPer } }

    function agregarOrdenMRP() {
        if (!_mrpDatos) { alert('⚠️ Primero calcula el MRP'); return; }
        const { material, lanzam, nb, lote, lt, modo, nPrev, nPer, stockIni } = _mrpDatos;

        // Si ya existe ese material, preguntar si reemplazar
        if (ordenesMRP[material]) {
            if (!confirm(`"${material}" ya tiene una orden calculada.\n¿Reemplazarla con el nuevo cálculo?`)) return;
        }

        ordenesMRP[material] = { ..._mrpDatos };

        // Notificación
        const btnAO = document.getElementById('btnAgregarOrden');
        if (btnAO) {
            btnAO.innerHTML = '<i class="fas fa-check"></i> Agregado!';
            btnAO.style.background = '#4ade80';
            btnAO.style.color = '#0a0e12';
            setTimeout(() => {
                btnAO.innerHTML = '<i class="fas fa-plus-circle"></i> Agregar a Órdenes';
                btnAO.style.background = '#1a5c2a';
                btnAO.style.color = 'white';
            }, 2000);
        }

        renderOrdenesAcumuladas();
    }

    function eliminarOrdenMRP(material) {
        if (!confirm(`¿Eliminar la orden de "${material}"?`)) return;
        delete ordenesMRP[material];
        renderOrdenesAcumuladas();
    }

    function renderOrdenesAcumuladas() {
        const el = document.getElementById('resultadoOrdenes');
        if (!el) return;

        const materiales = Object.keys(ordenesMRP);

        if (materiales.length === 0) {
            el.innerHTML = '<p style="color:#8bb3cc;font-size:0.85rem">📋 Calcula el MRP de cada material y presiona <strong>"Agregar a Órdenes"</strong> para acumularlos aquí.</p>';
            return;
        }

        const th = t => `<th style="background:#10323e;color:#a5f3fc;padding:4px 8px;font-size:0.75rem">${t}</th>`;
        const td = (v,c='') => `<td style="padding:3px 7px;text-align:right;font-size:0.75rem;${c?'color:'+c+';font-weight:bold':''}">${v}</td>`;
        const tl = t => `<td style="padding:3px 7px;font-size:0.75rem">${t}</td>`;

        let html2 = `<p style="color:#4ade80;font-size:0.8rem;margin-bottom:0.8rem">
            <i class="fas fa-check-circle"></i> <strong>${materiales.length}</strong> material(es) en el plan de órdenes
        </p>`;

        // Tabla resumen de lanzamientos
        html2 += `<div style="overflow-x:auto;margin-bottom:1rem">
        <table style="width:100%;border-collapse:collapse">
        <thead><tr>
            ${th('Material')}${th('Modo')}${th('Stock Ini')}${th('Lote')}${th('LT')}${th('Total NB')}${th('Total Pedido')}${th('Lanzamientos')}${th('Acciones')}
        </tr></thead><tbody>`;

        materiales.forEach(mat => {
            const d = ordenesMRP[mat];
            const inv = inventariosData.find(i => i.material === mat);
            const perLabel = i => i < d.nPrev
                ? (d.modo === 'semanas' ? `S-${d.nPrev-i}` : `M-${d.nPrev-i}`)
                : (d.modo === 'semanas' ? `S${i-d.nPrev+1}` : `M${i-d.nPrev+1}`);

            const totalNB  = d.nb.reduce((a,b)=>a+Math.max(0,b),0);
            const totalPed = d.pedidos.reduce((a,b)=>a+b,0);
            const lanzStr  = d.lanzam
                .map((v,i) => v > 0 ? `${perLabel(i)}: <strong>${v.toFixed(2)}</strong>` : '')
                .filter(Boolean).join(' | ') || '—';

            html2 += `<tr>
                ${tl(`<strong>${mat}</strong>`)}
                ${td(d.modo)}
                ${td(d.stockIni)}
                ${td(d.lote)}
                ${td(d.lt + ' per.')}
                ${td(totalNB.toFixed(2))}
                ${td(totalPed.toFixed(2), '#00f2fe')}
                <td style="padding:3px 7px;font-size:0.72rem">${lanzStr}</td>
                <td style="padding:3px 7px">
                    <button onclick="eliminarOrdenMRP('${mat.replace(/'/g,"\'")}')"
                        style="background:#883c2c;padding:0.2rem 0.5rem;margin:0;border-radius:0.4rem;font-size:0.7rem">
                        <i class="fas fa-trash"></i>
                    </button>
                </td>
            </tr>`;
        });

        html2 += `</tbody></table></div>`;

        // Detalle expandible por material
        html2 += `<p style="font-weight:700;color:#00f2fe;font-size:0.85rem;margin-bottom:0.5rem">Detalle por material:</p>`;

        materiales.forEach(mat => {
            const d = ordenesMRP[mat];
            const nTot = d.nb.length;
            const perLabel = i => i < d.nPrev
                ? (d.modo === 'semanas' ? `S-${d.nPrev-i}` : `M-${d.nPrev-i}`)
                : (d.modo === 'semanas' ? `S${i-d.nPrev+1}` : `M${i-d.nPrev+1}`);

            const mkFila = (label, arr, color='') =>
                `<tr><td style="padding:2px 6px;font-size:0.72rem;font-weight:600;${color?'color:'+color:''}">${label}</td>` +
                arr.map(v=>`<td style="padding:2px 5px;text-align:right;font-size:0.72rem">${typeof v==='number'?v.toFixed(2):v}</td>`).join('') +
                `</tr>`;

            html2 += `<details style="margin-bottom:0.5rem">
            <summary style="cursor:pointer;background:#0f1a1f;padding:0.4rem 0.8rem;border-radius:0.4rem;font-size:0.8rem;color:#00f2fe;list-style:none">
                ▶ ${mat} | LT: ${d.lt} | Lote: ${d.lote}
            </summary>
            <div style="overflow-x:auto;margin-top:0.3rem">
            <table style="width:100%;border-collapse:collapse;border:1px solid #2a4b5c">
            <thead><tr style="background:#10323e">
                <th style="padding:2px 6px;font-size:0.72rem;text-align:left;color:#a5f3fc">Concepto</th>
                ${Array.from({length:nTot},(_,i)=>`<th style="padding:2px 5px;font-size:0.72rem;color:#a5f3fc">${perLabel(i)}</th>`).join('')}
            </tr></thead><tbody>
            ${mkFila('Nec. Brutas',    d.nb)}
            ${mkFila('Entradas',       d.entradas)}
            ${mkFila('Stock Final',    d.stockFin)}
            ${mkFila('Nec. Netas',     d.nnetas.map(v=>Math.max(0,v)))}
            ${mkFila('Pedidos',        d.pedidos, '#c084fc')}
            ${mkFila('🚀 Lanzamiento', d.lanzam,  '#4ade80')}
            </tbody></table></div></details>`;
        });

        el.innerHTML = html2;
    }

    // ===============================================================
    // EOQ, ROP E INDICADORES DE INVENTARIO
    // ===============================================================
    let _eoqDatos = null;

    function poblarSelectEOQ() {
        const sel = document.getElementById('eoqMaterial');
        if (!sel) return;
        const prev = sel.value;
        sel.innerHTML = '<option value="">— Seleccionar —</option>';
        inventariosData.forEach(inv => {
            const opt = document.createElement('option');
            opt.value = inv.material;
            opt.textContent = inv.material;
            sel.appendChild(opt);
        });
        if (prev) sel.value = prev;
    }

    function autocompletarEOQ() {
        const mat = document.getElementById('eoqMaterial').value;
        if (!mat) return;
        const inv = inventariosData.find(i => i.material === mat);
        if (!inv) return;
        // Autocompletar Lead Time desde inventario
        if (inv.lt) document.getElementById('eoqL').value = inv.lt * 7; // semanas → días
        // Autocompletar lote como referencia
        if (inv.lote && inv.lote !== 'LFL') {
            document.getElementById('eoqD').placeholder = `Ref. lote: ${inv.lote}`;
        }
    }

    function calcularEOQ() {
        const D  = parseFloat(document.getElementById('eoqD').value);
        const S  = parseFloat(document.getElementById('eoqS').value);
        const C  = parseFloat(document.getElementById('eoqC').value);
        const i  = parseFloat(document.getElementById('eoqI').value) / 100;
        const L  = parseFloat(document.getElementById('eoqL').value);
        const dias = parseFloat(document.getElementById('eoqDias').value) || 264;
        const SS = parseFloat(document.getElementById('eoqSS').value) || 0;
        const NS = parseFloat(document.getElementById('eoqNS').value) || 95;
        const mat = document.getElementById('eoqMaterial').value || 'Material';

        if ([D,S,C,i,L].some(isNaN) || D<=0 || S<=0 || C<=0 || i<=0) {
            alert('⚠️ Completa D, S, C, i y Lead Time con valores positivos'); return;
        }

        const H   = C * i;                          // Costo mantener/unidad/año
        const EOQ = Math.sqrt((2 * D * S) / H);     // Cantidad óptima
        const ROP = (D / dias) * L + SS;            // Punto de reorden
        const nPedidos = D / EOQ;                   // Pedidos/año
        const tCiclo   = dias / nPedidos;            // Días entre pedidos
        const invProm  = EOQ / 2 + SS;              // Inventario promedio

        // Costos
        const costoOrden   = nPedidos * S;
        const costoMant    = invProm * H;
        const costoTotal   = costoOrden + costoMant;
        const costoSinEOQ  = (D / (EOQ*0.5)) * S + (EOQ*0.5/2 + SS) * H; // referencia

        // Ahorro vs lote arbitrario
        const ahorro = costoSinEOQ - costoTotal;

        _eoqDatos = { D, S, C, i, H, EOQ, ROP, SS, NS, nPedidos, tCiclo,
                      invProm, costoOrden, costoMant, costoTotal, dias, L, mat };

        const fmtC = v => `S/ ${v.toLocaleString('es-PE',{minimumFractionDigits:2,maximumFractionDigits:2})}`;
        const fmtN = (v, dec=2) => v.toLocaleString('es-PE',{minimumFractionDigits:dec,maximumFractionDigits:dec});

        // KPIs
        const kpis = [
            ['EOQ — Cantidad Óptima', fmtN(EOQ,1) + ' u.', '#00f2fe'],
            ['ROP — Punto de Reorden', fmtN(ROP,1) + ' u.', '#facc15'],
            ['Pedidos por año', fmtN(nPedidos,1), '#4ade80'],
            ['Ciclo de pedido', fmtN(tCiclo,0) + ' días', '#c084fc'],
            ['Inventario promedio', fmtN(invProm,1) + ' u.', '#4facfe'],
            ['Costo Total Anual', fmtC(costoTotal), '#f87171'],
            ['Costo de Ordenar', fmtC(costoOrden), '#8bb3cc'],
            ['Costo de Mantener', fmtC(costoMant), '#8bb3cc'],
            ['H (Costo mant./u./año)', fmtC(H), '#8bb3cc'],
            ['Nivel de Servicio', NS + '%', NS>=95?'#4ade80':'#facc15'],
        ];

        let html2 = `
        <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:0.6rem;margin-bottom:1rem">
            ${kpis.map(([label,val,color])=>`
            <div style="background:#0e2a33;border-radius:0.7rem;padding:0.7rem;text-align:center">
                <div style="font-size:0.68rem;color:#8bb3cc;margin-bottom:3px">${label}</div>
                <div style="font-size:1.1rem;font-weight:700;color:${color}">${val}</div>
            </div>`).join('')}
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-bottom:1rem">
            <!-- Fórmulas usadas -->
            <div style="background:#0f1a1f;border:1px solid #2a4b5c;border-radius:0.6rem;padding:0.8rem">
                <p style="font-weight:700;color:#00f2fe;font-size:0.8rem;margin-bottom:0.5rem">📐 Fórmulas Aplicadas</p>
                <div style="font-family:monospace;font-size:0.75rem;line-height:2">
                    <div>EOQ = √(2·D·S / H) = √(2·${D}·${S} / ${H.toFixed(4)})</div>
                    <div style="color:#00f2fe;font-weight:700">EOQ = <strong>${fmtN(EOQ,2)} unidades</strong></div>
                    <div style="margin-top:0.4rem">ROP = (D/días)·LT + SS</div>
                    <div>ROP = (${D}/${dias})·${L} + ${SS}</div>
                    <div style="color:#facc15;font-weight:700">ROP = <strong>${fmtN(ROP,2)} unidades</strong></div>
                    <div style="margin-top:0.4rem">H = C·i = ${C}·${(i*100).toFixed(1)}% = ${fmtC(H)}/u./año</div>
                    <div>N° Pedidos = D/EOQ = ${D}/${fmtN(EOQ,2)} = ${fmtN(nPedidos,2)}</div>
                    <div>Ciclo = ${dias}/${fmtN(nPedidos,2)} = ${fmtN(tCiclo,1)} días</div>
                </div>
            </div>
            <!-- Política de inventario -->
            <div style="background:#0f1a1f;border:1px solid #2a4b5c;border-radius:0.6rem;padding:0.8rem">
                <p style="font-weight:700;color:#00f2fe;font-size:0.8rem;margin-bottom:0.5rem">📋 Política de Inventario Recomendada</p>
                <div style="font-size:0.78rem;line-height:2">
                    <div>📦 <strong>Material:</strong> ${mat}</div>
                    <div>🛒 <strong>Pedir:</strong> ${fmtN(EOQ,1)} unidades cada vez</div>
                    <div>🚨 <strong>Reponer cuando:</strong> stock baje a ${fmtN(ROP,1)} u.</div>
                    <div>🛡️ <strong>Stock seguridad:</strong> ${SS} unidades</div>
                    <div>📅 <strong>Frecuencia:</strong> cada ${fmtN(tCiclo,0)} días (${fmtN(nPedidos,1)} veces/año)</div>
                    <div>💰 <strong>Costo anual total:</strong> ${fmtC(costoTotal)}</div>
                    <div style="color:#4ade80;margin-top:0.3rem">
                        ✅ Nivel de servicio objetivo: ${NS}%
                        ${NS>=95 ? '— Excelente cobertura' : NS>=85 ? '— Aceptable' : '— Revisar SS'}
                    </div>
                </div>
            </div>
        </div>

        <div class="ia-insight success">
            <i class="fas fa-robot"></i> <strong>IA EOQ:</strong>
            Con EOQ=${fmtN(EOQ,1)} u. el costo anual se minimiza a ${fmtC(costoTotal)}.
            El punto de reorden de ${fmtN(ROP,1)} u. garantiza cobertura durante el lead time de ${L} días.
            ${SS > 0 ? `El stock de seguridad de ${SS} u. protege contra variaciones de demanda.` : 'Considera agregar stock de seguridad para mayor confiabilidad.'}
        </div>`;

        document.getElementById('resultadoEOQ').innerHTML = html2;

        // Gráfico EOQ — Curva de costos
        if (charts.eoq) charts.eoq.destroy();
        const ctxEOQ = document.getElementById('chartEOQ').getContext('2d');
        const bgW = [{ id:'bgW', beforeDraw(c){const x=c.ctx;x.save();x.fillStyle='#ffffff';x.fillRect(0,0,c.width,c.height);x.restore();}}];

        // Generar curvas para Q = 0.1*EOQ a 3*EOQ
        const qMin = Math.max(1, EOQ * 0.1);
        const qMax = EOQ * 3;
        const nPts = 60;
        const qVals = Array.from({length:nPts},(_,k) => qMin + (qMax-qMin)*k/(nPts-1));
        const costoOrd  = qVals.map(q => (D/q)*S);
        const costoMan  = qVals.map(q => (q/2+SS)*H);
        const costoTot  = qVals.map((q,i) => costoOrd[i]+costoMan[i]);

        charts.eoq = new Chart(ctxEOQ, {
            type:'line', plugins:bgW,
            data:{
                labels: qVals.map(q=>q.toFixed(0)),
                datasets:[
                    {label:'Costo Ordenar (S/./año)',  data:costoOrd, borderColor:'#1A6FA8', borderWidth:2, pointRadius:0, tension:0.3},
                    {label:'Costo Mantener (S/./año)', data:costoMan, borderColor:'#E8A020', borderWidth:2, pointRadius:0, tension:0.3},
                    {label:'Costo Total (S/./año)',    data:costoTot, borderColor:'#f87171', borderWidth:3, pointRadius:0, tension:0.3},
                ]
            },
            options:{
                responsive:true,
                plugins:{
                    legend:{labels:{color:'#333'}},
                    title:{display:true,text:`Curva EOQ — ${mat} | Q* = ${fmtN(EOQ,1)} u.`,color:'#333',font:{size:13,weight:'bold'}},
                    annotation:{annotations:{
                        eoqLine:{type:'line',xMin:fmtN(EOQ,0),xMax:fmtN(EOQ,0),borderColor:'#4ade80',borderWidth:2,borderDash:[6,3]}
                    }}
                },
                scales:{
                    x:{ticks:{color:'#333',maxTicksLimit:10},title:{display:true,text:'Cantidad Q (unidades)',color:'#555'},grid:{color:'#eee'}},
                    y:{ticks:{color:'#333'},title:{display:true,text:'Costo Anual (S/.)',color:'#555'},grid:{color:'#eee'}}
                }
            }
        });

        // Línea vertical en EOQ
        const eoqIdx = qVals.findIndex(q => q >= EOQ);
        if (eoqIdx>=0) {
            charts.eoq.data.datasets.push({
                label:`EOQ = ${fmtN(EOQ,1)}`,
                data: Array(nPts).fill(null).map((_,k) => k===eoqIdx ? costoTot[k] : null),
                borderColor:'#4ade80', borderWidth:0,
                pointBackgroundColor:'#4ade80', pointRadius:8, pointStyle:'triangle',
                showLine:false
            });
            charts.eoq.update();
        }
    }

    // ── INDICADORES DE INVENTARIO ──────────────────────────────────
    function calcularIndicadores() {
        sincronizarInventarios();

        // Demanda anual desde PAP si existe
        const demAnual = _papDatos ? _papDatos.demandas.reduce((a,b)=>a+b,0) : 0;
        const invPromPAP = _papDatos ? _papDatos.p2?.invF?.reduce((a,b)=>a+b,0) / (_papDatos.n||12) : 0;

        // Inventario total actual
        const stockTotal = inventariosData.reduce((a,b)=>a+b.stock,0);
        const nMateriales = inventariosData.length;

        // Indicadores por material
        const indicadores = inventariosData.map(inv => {
            const rotacion = demAnual > 0 && inv.stock > 0 ? demAnual / inv.stock : 0;
            const diasInv  = rotacion > 0 ? 365 / rotacion : 999;
            const lotN     = parseFloat(inv.lote);
            const rop      = _eoqDatos && _eoqDatos.mat === inv.material ? _eoqDatos.ROP : (inv.lt || 0) * (demAnual/264);
            const estado   = inv.stock === 0 ? '🔴 Sin stock'
                           : inv.stock < rop  ? '🟡 Bajo ROP'
                           : '🟢 OK';
            return { ...inv, rotacion, diasInv, rop, estado };
        });

        // KPIs globales
        const sinStock   = indicadores.filter(i=>i.stock===0).length;
        const bajoPRO    = indicadores.filter(i=>i.stock>0&&i.stock<i.rop).length;
        const rotProm    = demAnual > 0 && stockTotal > 0 ? demAnual/stockTotal : 0;
        const diasProm   = rotProm > 0 ? 365/rotProm : 0;

        const fmtN = (v,d=2) => isFinite(v)&&v<9999 ? v.toLocaleString('es-PE',{minimumFractionDigits:d,maximumFractionDigits:d}) : '—';
        const th = t => `<th style="background:#10323e;color:#a5f3fc;padding:4px 8px;font-size:0.75rem">${t}</th>`;
        const td = (v,c='') => `<td style="padding:3px 7px;font-size:0.75rem;text-align:right;${c?'color:'+c+';font-weight:bold':''}">${v}</td>`;
        const tl = t => `<td style="padding:3px 7px;font-size:0.75rem">${t}</td>`;

        let html2 = `
        <!-- KPIs globales -->
        <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:0.5rem;margin-bottom:1rem">
            ${[
                ['Stock Total', stockTotal.toLocaleString('es-PE') + ' u.', '#00f2fe'],
                ['Materiales', nMateriales, '#4facfe'],
                ['Sin Stock', sinStock, sinStock>0?'#f87171':'#4ade80'],
                ['Bajo ROP', bajoPRO, bajoPRO>0?'#facc15':'#4ade80'],
                ['Rotación Global', demAnual>0?fmtN(rotProm,2)+'x':'—', '#c084fc'],
                ['Días Inventario', demAnual>0?fmtN(diasProm,0)+' d':'—', '#E8A020'],
            ].map(([l,v,c])=>`
            <div style="background:#0e2a33;border-radius:0.6rem;padding:0.6rem;text-align:center">
                <div style="font-size:0.67rem;color:#8bb3cc">${l}</div>
                <div style="font-size:1.1rem;font-weight:700;color:${c}">${v}</div>
            </div>`).join('')}
        </div>

        ${demAnual===0?'<div class="ia-insight warning">⚠️ Calcula el PAP primero para obtener la demanda anual y calcular rotación e indicadores de demanda.</div>':''}

        <!-- Tabla por material -->
        <div style="overflow-x:auto">
        <table style="width:100%;border-collapse:collapse">
        <thead><tr>
            ${th('Material')}${th('Und')}${th('Stock')}${th('Lote')}
            ${th('LT (sem)')}${th('ROP (u.)')}${th('Rotación')}${th('Días Inv.')}${th('Estado')}
        </tr></thead><tbody>
        ${indicadores.map(inv=>`<tr>
            ${tl(inv.material.length>30?inv.material.slice(0,28)+'...':inv.material)}
            ${td(inv.und)}
            ${td(inv.stock.toLocaleString(), inv.stock===0?'#f87171':'')}
            ${td(inv.lote)}
            ${td(inv.lt)}
            ${td(fmtN(inv.rop,1), inv.stock<inv.rop&&inv.stock>0?'#facc15':'')}
            ${td(demAnual>0?fmtN(inv.rotacion,2)+'x':'—')}
            ${td(demAnual>0&&inv.rotacion>0?fmtN(inv.diasInv,0)+' d':'—')}
            ${td(inv.estado)}
        </tr>`).join('')}
        </tbody></table></div>

        <div class="ia-insight ${sinStock>0?'danger':bajoPRO>0?'warning':'success'}" style="margin-top:0.8rem">
        <i class="fas fa-robot"></i> <strong>IA Inventarios:</strong>
        ${sinStock>0 ? `🔴 ${sinStock} material(es) sin stock — riesgo de paro de producción inmediato.` :
          bajoPRO>0  ? `🟡 ${bajoPRO} material(es) por debajo del punto de reorden — generar órdenes urgentes.` :
          '✅ Todos los materiales están por encima de su punto de reorden. Inventario saludable.'}
        ${demAnual>0 ? ` Rotación global: ${fmtN(rotProm,2)}x/año (${fmtN(diasProm,0)} días de inventario).` : ''}
        </div>`;

        document.getElementById('resultadoIndicadores').innerHTML = html2;

        // Gráfico indicadores — barras de stock vs ROP
        if (charts.ind) charts.ind.destroy();
        const ctxInd = document.getElementById('chartIndicadores').getContext('2d');
        const bgW = [{ id:'bgW', beforeDraw(c){const x=c.ctx;x.save();x.fillStyle='#ffffff';x.fillRect(0,0,c.width,c.height);x.restore();}}];
        const labels = indicadores.map(i => i.material.length>18?i.material.slice(0,16)+'..':i.material);
        const stocks = indicadores.map(i => i.stock);
        const rops   = indicadores.map(i => i.rop);
        charts.ind = new Chart(ctxInd, {
            type:'bar', plugins:bgW,
            data:{
                labels,
                datasets:[
                    {label:'Stock Actual', data:stocks,
                     backgroundColor: stocks.map((s,i)=>s===0?'rgba(248,113,113,0.8)':s<rops[i]?'rgba(250,204,21,0.8)':'rgba(74,222,128,0.8)'),
                     borderWidth:1},
                    {label:'Punto de Reorden (ROP)', data:rops,
                     type:'line', borderColor:'#f87171', borderWidth:2, borderDash:[5,4],
                     pointBackgroundColor:'#f87171', pointRadius:4, tension:0}
                ]
            },
            options:{
                responsive:true,
                plugins:{
                    legend:{labels:{color:'#333'}},
                    title:{display:true,text:'Stock Actual vs Punto de Reorden (ROP)',color:'#333',font:{size:13,weight:'bold'}}
                },
                scales:{
                    x:{ticks:{color:'#333',maxRotation:45},grid:{color:'#eee'}},
                    y:{ticks:{color:'#333'},title:{display:true,text:'Unidades',color:'#555'},grid:{color:'#eee'}}
                }
            }
        });
    }

    function exportarExcelEOQ() {
        if (!_eoqDatos) { alert("Primero calcula el EOQ"); return; }
        const { D, S, C, i, H, EOQ, ROP, SS, nPedidos, tCiclo, invProm,
                costoOrden, costoMant, costoTotal, dias, L, mat } = _eoqDatos;
        const cells = [];
        let r = 0;
        cells.push(ct(0, r++, 'Sistema MRP II — Leonardo Carrasco Ocon'));
        cells.push(ct(0, r++, 'EOQ — Cantidad Económica de Pedido'));
        r++;
        cells.push(ct(0, r, 'Material')); cells.push(ct(1, r++, mat));
        cells.push(ct(0, r, 'Parámetro')); cells.push(ct(1, r, 'Símbolo'));
        cells.push(ct(2, r++, 'Valor'));
        const params = [
            ['Demanda anual','D', D],
            ['Costo por orden','S', S],
            ['Costo unitario','C', C],
            ['Tasa mantenimiento','i', i],
            ['Costo mantenimiento/u./año','H=C×i', H],
            ['Lead Time (días)','L', L],
            ['Días laborables/año','días', dias],
            ['Stock de seguridad','SS', SS],
        ];
        params.forEach(([label,sym,val]) => {
            cells.push(ct(0, r, label)); cells.push(ct(1, r, sym));
            cells.push(cn(2, r++, val));
        });
        r++;
        cells.push(ct(0, r, 'RESULTADOS')); r++;
        const resultados = [
            ['EOQ — Cantidad Óptima', EOQ],
            ['ROP — Punto de Reorden', ROP],
            ['Número de pedidos/año', nPedidos],
            ['Ciclo de pedido (días)', tCiclo],
            ['Inventario promedio', invProm],
            ['Costo anual ordenar', costoOrden],
            ['Costo anual mantener', costoMant],
            ['Costo Total Anual', costoTotal],
        ];
        const dS = r;
        resultados.forEach(([label,val]) => {
            cells.push(ct(0, r, label)); cells.push(cn(1, r++, Number(val.toFixed(4))));
        });
        r++;
        // Fórmulas
        cells.push(ct(0, r, 'Fórmula EOQ'));
        cells.push(cf(1, r, `SQRT(2*C3*C4/C7)`, Number(EOQ.toFixed(4))));
        r++;
        cells.push(ct(0, r, 'Fórmula ROP'));
        cells.push(cf(1, r, `(C3/C11)*C10+C12`, Number(ROP.toFixed(4))));
        r++;
        cells.push(ct(0, r, 'Fórmula Costo Total'));
        cells.push(cf(1, r, `(C3/C${dS+1})*C4+(C${dS+1}/2+C12)*C7`, Number(costoTotal.toFixed(4))));
        const ws = construirHoja(cells, 3, r+1);
        ws['!cols'] = [32,12,14].map(w=>({wch:w}));
        descargarExcel(`EOQ_${mat.replace(/ /g,'_')}`, 'EOQ', ws);
    }

    // ================= INICIALIZACIÓN =================
    // ===============================================================
    // SISTEMA DE SESIÓN — localStorage
    // ===============================================================
    const SESION_KEY = 'mrp2_sesion_v1';

    function recolectarInputs() {
        // Recoge todos los inputs y selects del sistema con su id y valor
        const datos = {};
        document.querySelectorAll('input[id], select[id], textarea[id]').forEach(el => {
            if (el.id) datos[el.id] = el.value;
        });
        return datos;
    }

    function guardarSesion() {
        sincronizarInventarios();
        const sesion = {
            fecha:      new Date().toISOString(),
            inputs:     recolectarInputs(),
            inventarios: inventariosData.map(i => ({...i})),
            bom:         bomData.map(b => ({...b})),
            compras:     comprasData.map(c => ({...c})),
            portada: {
                autor:    document.getElementById('portadaAutor')?.value  || '',
                empresa:  document.getElementById('portadaEmpresa')?.value || '',
                curso:    document.getElementById('portadaCurso')?.value   || '',
                profesor: document.getElementById('portadaProfesor')?.value || '',
                periodo:  document.getElementById('portadaPeriodo')?.value  || '',
                fecha:    document.getElementById('portadaFecha')?.value    || '',
            }
        };
        try {
            localStorage.setItem(SESION_KEY, JSON.stringify(sesion));
            const ahora = new Date().toLocaleString('es-PE');
            document.getElementById('sesionEstado').textContent = '✅ Guardado: ' + ahora;
            document.getElementById('sesionEstado').style.color = '#4ade80';
            // Auto-guardar también en 3 segundos para confirmar
            setTimeout(() => {
                document.getElementById('sesionEstado').textContent = '💾 Sesión guardada automáticamente';
                document.getElementById('sesionEstado').style.color = '#8bb3cc';
            }, 3000);
        } catch(e) {
            alert('⚠️ No se pudo guardar: ' + e.message);
        }
    }

    function cargarSesion() {
        try {
            const raw = localStorage.getItem(SESION_KEY);
            if (!raw) {
                alert('⚠️ No hay sesión guardada. Guarda primero tus datos con "Guardar sesión".');
                return;
            }
            const sesion = JSON.parse(raw);
            const fecha  = new Date(sesion.fecha).toLocaleString('es-PE');

            if (!confirm(`¿Cargar la sesión guardada el ${fecha}?
Se reemplazarán los datos actuales.`)) return;

            // Restaurar inputs
            if (sesion.inputs) {
                Object.entries(sesion.inputs).forEach(([id, val]) => {
                    const el = document.getElementById(id);
                    if (el && !id.startsWith('nb_') && !id.startsWith('bom_') && !id.startsWith('mat_')
                           && !id.startsWith('stock_') && !id.startsWith('lote_') && !id.startsWith('lt_')
                           && !id.startsWith('und_')) {
                        el.value = val;
                    }
                });
            }

            // Restaurar inventarios
            if (sesion.inventarios && sesion.inventarios.length) {
                sesion.inventarios.forEach((inv, i) => {
                    if (i < inventariosData.length) Object.assign(inventariosData[i], inv);
                });
                mostrarTablaInventarios();
            }

            // Restaurar BOM
            if (sesion.bom && sesion.bom.length) {
                bomData.length = 0;
                sesion.bom.forEach(b => bomData.push(b));
                mostrarBOM();
            }

            // Restaurar compras
            if (sesion.compras) {
                comprasData.length = 0;
                sesion.compras.forEach(c => comprasData.push(c));
                renderTablaCompras();
            }

            // Restaurar portada
            if (sesion.portada) {
                const p = sesion.portada;
                if (document.getElementById('portadaAutor'))   document.getElementById('portadaAutor').value   = p.autor    || '';
                if (document.getElementById('portadaEmpresa')) document.getElementById('portadaEmpresa').value = p.empresa  || '';
                if (document.getElementById('portadaCurso'))   document.getElementById('portadaCurso').value   = p.curso    || '';
                if (document.getElementById('portadaProfesor'))document.getElementById('portadaProfesor').value= p.profesor || '';
                if (document.getElementById('portadaPeriodo')) document.getElementById('portadaPeriodo').value = p.periodo  || '';
                if (document.getElementById('portadaFecha'))   document.getElementById('portadaFecha').value   = p.fecha    || '';
            }

            // Refrescar MRP y órdenes
            poblarSelectMRP();
            generarInputsMRP();
            generarOrdenesAprovisionamiento();
            actualizarERP();

            document.getElementById('sesionEstado').textContent = '📂 Sesión cargada: ' + fecha;
            document.getElementById('sesionEstado').style.color = '#4ade80';
            alert('✅ Sesión cargada correctamente. Recalcula los módulos (PAP, PMP, MRP) para ver los resultados.');
        } catch(e) {
            alert('⚠️ Error al cargar la sesión: ' + e.message);
        }
    }

    function borrarSesion() {
        if (!confirm('¿Borrar la sesión guardada? Esta acción no se puede deshacer.')) return;
        localStorage.removeItem(SESION_KEY);
        document.getElementById('sesionEstado').textContent = '🗑️ Sesión borrada';
        document.getElementById('sesionEstado').style.color = '#f87171';
        setTimeout(() => {
            document.getElementById('sesionEstado').textContent = '';
        }, 3000);
    }

    function autoGuardar() {
        // Auto-guardado silencioso cada 60 segundos
        try {
            const raw = localStorage.getItem(SESION_KEY);
            // Solo auto-guarda si ya existe una sesión previa (el usuario guardó explícitamente)
            if (raw) {
                guardarSesion();
                document.getElementById('sesionEstado').textContent = '💾 Auto-guardado';
                document.getElementById('sesionEstado').style.color = '#8bb3cc';
            }
        } catch(e) {}
    }

    function verificarSesionGuardada() {
        try {
            const raw = localStorage.getItem(SESION_KEY);
            if (raw) {
                const sesion = JSON.parse(raw);
                const fecha  = new Date(sesion.fecha).toLocaleString('es-PE');
                document.getElementById('sesionEstado').textContent = '💾 Sesión disponible: ' + fecha;
                document.getElementById('sesionEstado').style.color = '#facc15';
            }
        } catch(e) {}
    }

    function init() {
        mostrarTablaInventarios();
        mostrarBOM();
        cargarSKUsdesdeBOM(); // cargar SKUs dinámicos desde BOM al inicio

        document.getElementById('btnPM').addEventListener('click', calcularPM);
        document.getElementById('btnExcelPM').addEventListener('click', exportarExcelPM);

        document.getElementById('btnSE').addEventListener('click', calcularSE);
        document.getElementById('btnExcelSE').addEventListener('click', exportarExcelSE);

        document.getElementById('btnReg').addEventListener('click', calcularReg);
        document.getElementById('btnExcelReg').addEventListener('click', exportarExcelReg);

        document.getElementById('btnPAP').addEventListener('click', calcularPAP);
        document.getElementById('btnExcelPAP').addEventListener('click', exportarExcelPAP);

        document.getElementById('btnPMP').addEventListener('click', () => { calcularPMP(); generarOrdenesAprovisionamiento(); });
        document.getElementById('btnPMPdesdeBOM').addEventListener('click', cargarSKUsdesdeBOM);
        document.getElementById('btnExcelPMP').addEventListener('click', exportarExcelPMP);

        document.getElementById('btnAgregarInv').addEventListener('click', agregarFilaInventario);
        document.getElementById('btnGuardarInv').addEventListener('click', () => { guardarInventarios(); generarOrdenesAprovisionamiento(); });
        document.getElementById('btnExcelInv').addEventListener('click', exportarExcelInventarios);

        document.getElementById('btnExcelBOM').addEventListener('click', exportarExcelBOM);
        document.getElementById('btnEditarBOM').addEventListener('click', () => {
            editandoBOM = !editandoBOM;
            mostrarBOM();
        });
        document.getElementById('btnGuardarBOM').addEventListener('click', guardarBOM);

        document.getElementById('btnMRP').addEventListener('click', calcularMRP);
        document.getElementById('btnAgregarOrden').addEventListener('click', agregarOrdenMRP);
        document.getElementById('btnExcelMRP').addEventListener('click', exportarExcelMRP);
        document.getElementById('btnLimpiarMRP').addEventListener('click', () => {
            const nPer  = parseInt(document.getElementById('nPeriodosMRP').value) || 4;
            const nPrev = parseInt(document.getElementById('periodosPrevMRP').value) || 0;
            for (let i = 0; i < nPrev; i++) { const el = document.getElementById(`nb_prev_${i}`); if(el) el.value = 0; }
            for (let i = 0; i < nPer;  i++) { const el = document.getElementById(`nb_act_${i}`);  if(el) el.value = ''; }
        });
        // Inicializar campos MRP al cargar
        poblarSelectMRP();
        generarInputsMRP();
        document.getElementById('btnSyncMRP').addEventListener('click', () => {
            sincronizarInventarios();
            poblarSelectMRP();
            generarInputsMRP();
            alert('✅ Lista de materiales actualizada desde Inventarios');
        });

        document.getElementById('btnExportarOrdenes').addEventListener('click', exportarOrdenesCSV);
        document.getElementById('btnExcelOrdenes').addEventListener('click', exportarExcelOrdenes);
        document.getElementById('btnExportarPDF').addEventListener('click', exportarPDF);

        // ── MRP II listeners ──────────────────────────────────────────
        document.getElementById('btnCRP').addEventListener('click', calcularCRP);
        document.getElementById('btnCRPdesdeMRP').addEventListener('click', () => {
            if (_mrpDatos && _mrpDatos.nb) {
                const nPer = _mrpDatos.nPer || 4;
                const prod = _mrpDatos.nb.slice(-nPer).map(v=>Math.max(0,v));
                document.getElementById('crpSemanas').value  = nPer;
                document.getElementById('crpProdSem').value  = prod.join(',');
                alert('✅ Producción cargada desde MRP: ' + prod.join(', ') + ' pares/semana');
            } else { alert('⚠️ Primero calcula el MRP'); }
        });
        document.getElementById('btnExcelCRP').addEventListener('click', () => alert('Exportar CRP a Excel — próximamente'));

        document.getElementById('btnSFC').addEventListener('click', calcularSFC);
        document.getElementById('btnExcelSFC').addEventListener('click', () => alert('Exportar Control Planta a Excel — próximamente'));

        document.getElementById('btnGenerarCompras').addEventListener('click', generarComprasDesdeOrdenes);
        document.getElementById('btnAgregarCompra').addEventListener('click', agregarFilaCompra);
        document.getElementById('btnExcelCompras').addEventListener('click', () => alert('Exportar Compras a Excel — próximamente'));

        document.getElementById('btnFinanciero').addEventListener('click', calcularFinanciero);
        document.getElementById('btnFinDesdePAP').addEventListener('click', () => {
            if (_papDatos) {
                alert('✅ Datos de PAP cargados. Completa los campos de precio y costos unitarios para calcular.');
            } else { alert('⚠️ Primero calcula el PAP'); }
        });
        document.getElementById('btnExcelFinanciero').addEventListener('click', () => alert('Exportar Financiero a Excel — próximamente'));

        // ── EOQ & Indicadores ─────────────────────────────────────────
        poblarSelectEOQ();
        document.getElementById('btnEOQ').addEventListener('click', calcularEOQ);
        document.getElementById('btnIndicadores').addEventListener('click', calcularIndicadores);
        document.getElementById('btnEOQdesdeMRP').addEventListener('click', () => {
            if (_mrpDatos) {
                const { nb, material, lt } = _mrpDatos;
                const demSem = nb.reduce((a,b)=>a+Math.max(0,b),0);
                const demAnual = demSem * (52 / (_mrpDatos.nPer||4));
                document.getElementById('eoqMaterial').value = material;
                document.getElementById('eoqD').value = demAnual.toFixed(0);
                document.getElementById('eoqL').value = (lt * 7).toFixed(0);
                autocompletarEOQ();
                alert(`✅ Cargado desde MRP:\nMaterial: ${material}\nDemanda estimada: ${demAnual.toFixed(0)} u./año\nLead Time: ${lt*7} días`);
            } else { alert('⚠️ Primero calcula el MRP'); }
        });
        document.getElementById('btnEnviarROP').addEventListener('click', () => {
            if (!_eoqDatos) { alert('⚠️ Primero calcula el EOQ'); return; }
            const { ROP, EOQ, mat } = _eoqDatos;
            // Actualizar stock de seguridad en inventariosData
            const inv = inventariosData.find(i => i.material === mat);
            if (inv) {
                // Actualizar el input de stock del material en la tabla
                const idx = inventariosData.indexOf(inv);
                const stockEl = document.getElementById(`stock_${idx}`);
                if (stockEl && parseFloat(stockEl.value) < ROP) {
                    if (confirm(`El ROP calculado es ${ROP.toFixed(1)} u.\n¿Actualizar el stock mínimo de "${mat}" en Inventarios?`)) {
                        stockEl.value = Math.ceil(ROP);
                        guardarInventarios();
                        alert(`✅ ROP ${ROP.toFixed(1)} aplicado como stock referencia en Inventarios.\nEOQ recomendado: ${EOQ.toFixed(1)} u. por pedido.`);
                    }
                } else {
                    alert(`ℹ️ ROP: ${ROP.toFixed(1)} u. | EOQ: ${EOQ.toFixed(1)} u.\nEl stock actual ya supera el ROP.\nRecuerda pedir EOQ unidades cuando el stock llegue al ROP.`);
                }
            } else {
                alert(`ROP: ${ROP.toFixed(1)} u. | EOQ: ${EOQ.toFixed(1)} u.\nAgrega "${mat}" al inventario para aplicar el ROP automáticamente.`);
            }
        });
        document.getElementById('btnExcelEOQ').addEventListener('click', exportarExcelEOQ);
        document.getElementById('btnFinDesdePAP').addEventListener('click', () => {
            if (_papDatos) {
                alert('✅ Datos de PAP cargados. Completa los campos de precio y costos unitarios para calcular.');
            } else { alert('⚠️ Primero calcula el PAP'); }
        });
        document.getElementById('btnExcelFinanciero').addEventListener('click', () => alert('Exportar Financiero a Excel — próximamente'));

        renderOrdenesAcumuladas();
        generarOrdenesAprovisionamiento();

        // ── ERP, Respaldo, Portada ────────────────────────────────────
        document.getElementById('btnERPActualizar').addEventListener('click', actualizarERP);
        document.getElementById('btnERPCaptura').addEventListener('click', async () => {
            const el = document.getElementById('erpContainer');
            const canvas = await html2canvas(el, { scale:2, backgroundColor:'#f5f5f0' });
            const link = document.createElement('a');
            link.href = canvas.toDataURL('image/png');
            link.download = 'ERP_Captura_' + new Date().toISOString().slice(0,10) + '.png';
            link.click();
        });
        document.getElementById('btnExportarRespaldo').addEventListener('click', async () => {
            const el = document.getElementById('tab15');
            const canvas = await html2canvas(el, { scale:2, backgroundColor:'#0a0e12' });
            const { jsPDF } = window.jspdf;
            const pdf = new jsPDF('p','mm','a4');
            const iw = 210; const ih = (canvas.height*210)/canvas.width;
            pdf.addImage(canvas.toDataURL('image/png'),'PNG',0,0,iw,ih);
            pdf.save('Material_Respaldo_MRP2.pdf');
        });
        document.getElementById('btnPortadaPDF').addEventListener('click', async () => {
            const el = document.getElementById('portadaContainer');
            const canvas = await html2canvas(el, { scale:2, backgroundColor:'#0a0e12' });
            const { jsPDF } = window.jspdf;
            const pdf = new jsPDF('p','mm','a4');
            const iw = 210; const ih = (canvas.height*210)/canvas.width;
            pdf.addImage(canvas.toDataURL('image/png'),'PNG',0,0,iw,ih);
            pdf.save('Portada_MRP2.pdf');
        });

        // Inicializar ERP, Respaldo y Portada
        actualizarERP();
        renderRespaldo();
        inicializarPortada();

        // ── Sistema de Sesión ─────────────────────────────────────────
        document.getElementById('btnGuardarSesion').addEventListener('click', guardarSesion);
        document.getElementById('btnCargarSesion').addEventListener('click', cargarSesion);
        document.getElementById('btnBorrarSesion').addEventListener('click', borrarSesion);

        // Verificar si hay sesión guardada al cargar
        verificarSesionGuardada();

        // Auto-guardado cada 60 segundos (solo si ya existe sesión previa)
        setInterval(autoGuardar, 60000);

        // Guardar sesión automáticamente al cerrar/recargar la página
        window.addEventListener('beforeunload', () => {
            try {
                const raw = localStorage.getItem(SESION_KEY);
                if (raw) guardarSesion(); // solo si ya guardó antes manualmente
            } catch(e) {}
        });
    }

    // Pestañas
    document.querySelectorAll('.tab-btn').forEach(btn => {
        btn.addEventListener('click', () => {
            document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));
            document.querySelectorAll('.tab-panel').forEach(p => p.classList.remove('active'));
            btn.classList.add('active');
            document.getElementById(btn.dataset.tab).classList.add('active');
        });
    });

    init();
</script>
</body>
</html>
