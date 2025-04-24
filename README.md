graph TD
    P{project structure}
    P --> C(project)
    P --> H(create_app)
    P --> WER(report_app)
    P --> M(main_app)
    P --> U(user_app)

    C --> C1[login_manager.py]
    C --> C2[__init__.py]
    C --> C3[settings.py]
    C --> C4[urls.py]
    C --> C5(templates)
    C5 --> M1[base.html]
    C --> C6(static)
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

    WER --> WER1[__init__.py]
    WER --> WER2[models.py]
    WER --> WER3[views.py]
    WER --> VOD(templates)
    VOD --> VOD1[report.html]
    WER --> SVO(static)
    SVO --> OVS(images)
    SVO --> OVS1(css)
    OVS1 --> OVSZ[report.css]

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


