# abwert
graph TD
    %% Корень проекта
    Root[Root] --> A[(app.py)]
    Root --> C[project]
    Root --> H[create_app]
    Root --> I[report_app]
    Root --> J[auth]
    Root --> D[static]
    Root --> E[templates]
    Root --> B[IMAGES]
    Root --> F[new_icons]
    Root --> G[tests]

    %% Папка project
    C --> C1[(app_manager.py)]
    C --> C2[(__init__.py)]
    C --> C3[(settings.py)]
    C --> C4[(utils.py)]

    %% Папка create_app
    H --> H1[(__init__.py)]
    H --> H2[(create.py)]
    H --> H3[(views.py)]

    %% Папка report_app
    I --> I1[(__init__.py)]
    I --> I2[(reports.py)]
    I --> I3[(views.py)]

    %% Папка auth
    J --> J1[(__init__.py)]
    J --> J2[(auth.py)]
    J --> J3[(forms.py)]

    %% Папка static
    D --> D1[(background.png)]
    D --> D2[(style.css)]
    D --> D3[(book.png)]

    %% Папка templates
    E --> E1[(base.html)]

    %% Папка IMAGES
    B --> B1[(settings.png)]
    B --> B2[(create.png)]
    B --> B3[(Background.png)]
    B --> B4[(profile.png)]
    B --> B5[(report.png)]

    %% Папка new_icons
    F --> F1[(create.png)]
    F --> F2[(report.png)]
    F --> F3[(profile.png)]
    F --> F4[(main.png)]
    F --> F5[(settings.png)]
