graph TD
    P{project structure}
    P --> C(project)
    P --> H(create_app)
    P --> WER(report_app)
    P --> M(main_app)
    P --> U(user_app)

    %% project folder
    C --> C1[login_manager.py]
    C --> C2[__init__.py]
    C --> C3[settings.py]
    C --> C4[urls.py]
    C --> C5(templates)
    C --> C6(static)
    C5 --> M1[base.html]
    C6 --> SW[background.png]
    C6 --> SW1[book.png]
    C6 --> SW2[style.css]
    C6 --> IC[icon.png]
    C6 --> IMAGES(images)
    IMAGES --> WSA[profile.png]
    IMAGES --> WSA1[main.png]
    IMAGES --> WSA2[settings.png]
    IMAGES --> WSA3[tests.png]
    IMAGES --> WSA4[report.png]
    IMAGES --> WSA5[create.png]

    %% create_app folder
    H --> H1[__init__.py]
    H --> H2[models.py]
    H --> H3[views.py]
    H --> H4[app.py]
    H --> ST(static)
    ST --> IM(images)
    ST --> CSSZ(css)
    CSSZ --> CREATCSS[create.css]
    H --> HTEM(templates)
    HTEM --> HTEM1[report.html]

    %% report_app folder
    WER --> WER1[__init__.py]
    WER --> WER2[models.py]
    WER --> WER3[views.py]
    WER --> VOD(templates)
    VOD --> VOD1[report.html]
    WER --> SVO(static)
    SVO --> OVS(images)
    SVO --> OVS1(css)
    OVS1 --> OVSZ[report.css]

    %% main_app folder
    M --> A[app.py]
    M --> I[__init__.py]
    M --> V[views.py]
    M --> T(templates)
    M --> S(static)
    S --> CER(css)
    CER --> MAI[main.css]
    S --> IM2(images)
    IM2 --> UK[ukr.png]
    IM2 --> CH[chemistry.png]
    IM2 --> MTH[math.png]
    IM2 --> E[end.png]
    IM2 --> PH[physic.png]
    IM2 --> PY[python.png]
    T --> MA[main.html]

    %% user_app folder
    U --> VI[views.py]
    U --> AP[app.py]
    U --> MO[models.py]
    U --> IN[__init__.py]
    U --> TE(templates)
    TE --> UH[user.html]
    TE --> PHE[personal.html]
    U --> ST2(static)
    ST2 --> J(js)
    J --> SJ[script.js]
    ST2 --> CS(css)
    CS --> UC[user.css]

    %% Styling
    classDef folder fill:#f9f,stroke:#333,stroke-width:2px;
    classDef file fill:#bbf,stroke:#333,stroke-width:1px;

    class P,C,H,WER,M,U,C5,C6,ST,HTEM,VOD,SVO,T,S,TE,ST2,IMAGES,IM,OVS,OVS1,CER,IM2,J,CS folder;
    class C1,C2,C3,C4,M1,SW,SW1,SW2,IC,WSA,WSA1,WSA2,WSA3,WSA4,WSA5,H1,H2,H3,H4,HTEM1,CREATCSS,WER1,WER2,WER3,VOD1,OVSZ,A,I,V,MA,UK,CH,MTH,E,PH,PY,VI,AP,MO,IN,UH,PHE,SJ,UC file;


