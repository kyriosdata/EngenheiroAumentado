## Visão geral de hemogramas

- Profa. Ana Laura ([vídeo](https://drive.google.com/file/d/11Mu27n1Av6A4__0fBmQ-vCtoo64JtKyJ/view?usp=drive_link))
  
## Ideia de negócio: monitoramento de hemogramas

A Secretaria de Estado de Saúde de Goiás (SES-GO) estará recebendo,
em tempo real, hemogramas
de laboratórios em território goiano. A expectativa é 
que sejam recebidos, quando todo o processo estiver
em pleno funcionamento, cerca de 65.000 hemogramas 
por dia.

Conforme abaixo, várias informações relevantes 
são úteis e podem ser obtidas dos hemogramas
de uma população, além, naturalmente, do uso 
individual:

1. Critérios de Hemoglobina para Anemia:
A OMS estabeleceu valores de referência padronizados para diferentes grupos populacionais (crianças, mulheres grávidas, mulheres não-grávidas, homens) para identificar anemia em nível comunitário.

2. Vigilância Comunitária:
A anemia afeta cerca de 25% da população mundial, com maior impacto em mulheres e crianças Emerging Point-of-Care Technologies for Anemia Detection - PMC, tornando essencial o desenvolvimento de ferramentas de detecção em nível comunitário.
3. Tecnologias Point-of-Care:
A OMS promove o uso de dispositivos de diagnóstico rápido para hemograma em cenários comunitários. Estudos mostram a precisão diagnóstica de dispositivos point-of-care para detecção de anemia em configurações comunitárias Diagnostic accuracy of point-of-care devices for detection of anemia in community settings in India | BMC Health Services Research.

Os hemogramas serão recebidos pela SES-GO por meio do padrão FHIR e 
estarão registrados por meio de instâncias de recursos Observation em JSON. A intenção é implementar um Sistema de Vigilância Populacional ou um CDSS (Clinical Decision Support System) que gere alertas
para gestores ou individualmente para os profissionais que assistem um indivíduo.
