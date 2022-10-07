ENACT R01 Analysis
================
Jiayuan Shi
2022-10-03

    ## Loading required package: lattice

    ## Loading required package: survival

    ## Loading required package: Formula

    ## Loading required package: ggplot2

    ## 
    ## Attaching package: 'Hmisc'

    ## The following objects are masked from 'package:base':
    ## 
    ##     format.pval, units

### Demographic, Recruitment Tracking, Telephone MOCA

Overall:

    ## 
    ## Attaching package: 'table1'

    ## The following objects are masked from 'package:Hmisc':
    ## 
    ##     label, label<-, units

    ## The following objects are masked from 'package:base':
    ## 
    ##     units, units<-

    ##                                 Overall
    ## 1                              (N=1127)
    ## 2 redcap_event_name.factor             
    ## 3                Screening 1090 (96.7%)
    ## 4                 Baseline    37 (3.3%)
    ## 5               Six months       0 (0%)

Screening:

    ##                                                       Overall
    ## 1                                                    (N=1090)
    ## 2                               site.factor                  
    ## 3                                   Boulder       561 (51.5%)
    ## 4                             Denver Health       529 (48.5%)
    ## 5                               AF Williams            0 (0%)
    ## 6                         Lone Tree Primary            0 (0%)
    ## 7                         Anschutz Internal            0 (0%)
    ## 8                            Lowry Internal            0 (0%)
    ## 9                                  Clinic 7            0 (0%)
    ## 10                                 Clinic 8            0 (0%)
    ## 11                                 Clinic 9            0 (0%)
    ## 12                                Clinic 10            0 (0%)
    ## 13                                      Age                  
    ## 14                                Mean (SD)       76.9 (5.65)
    ## 15                        Median [Min, Max]  75.5 [70.1, 103]
    ## 16                          language.factor                  
    ## 17                                  English       811 (74.4%)
    ## 18                                  Spanish       279 (25.6%)
    ## 19                     Prefer not to answer            0 (0%)
    ## 20                              race.factor                  
    ## 21                                    White       928 (85.1%)
    ## 22                   African American/Black         26 (2.4%)
    ## 23                                    Asian         18 (1.7%)
    ## 24   Native Hawaiian/Other Pacific Islander          2 (0.2%)
    ## 25           American Indian/Alaskan Native         11 (1.0%)
    ## 26                                    Other         94 (8.6%)
    ## 27                     Prefer not to answer         11 (1.0%)
    ## 28                         ethnicity.factor                  
    ## 29                             Not Hispanic       658 (60.4%)
    ## 30                                 Hispanic       426 (39.1%)
    ## 31                          Unknown/Refused          6 (0.6%)
    ## 32                            gender.factor                  
    ## 33                                     Male       517 (47.4%)
    ## 34                                   Female       573 (52.6%)
    ## 35                               Non-binary            0 (0%)
    ## 36                              Transgender            0 (0%)
    ## 37                        None of the above            0 (0%)
    ## 38                     Prefer not to answer            0 (0%)
    ## 39     ehr_demographic_data_complete.factor                  
    ## 40                               Incomplete            0 (0%)
    ## 41                               Unverified            0 (0%)
    ## 42                                 Complete       1090 (100%)
    ## 43     recruitment_tracking_complete.factor                  
    ## 44                               Incomplete       857 (78.6%)
    ## 45                               Unverified            0 (0%)
    ## 46                                 Complete       233 (21.4%)
    ## 47                 Raw Telephone MOCA score                  
    ## 48                                Mean (SD)       19.0 (2.44)
    ## 49                        Median [Min, Max] 20.0 [12.0, 22.0]
    ## 50                                  Missing      1051 (96.4%)
    ## 51           Corrected Telephone MOCA score                  
    ## 52                                Mean (SD)       19.0 (2.44)
    ## 53                        Median [Min, Max] 20.0 [12.0, 22.0]
    ## 54                                  Missing      1051 (96.4%)
    ## 55                         rand_moca.factor                  
    ## 56             1 - Less than or equal to 17          7 (0.6%)
    ## 57                      2 - Greater than 17         32 (2.9%)
    ## 58                                  Missing      1051 (96.4%)
    ## 59                      caregiver_yn.factor                  
    ## 60                                      Yes          1 (0.1%)
    ## 61                                       No          8 (0.7%)
    ## 62                                  Missing      1081 (99.2%)
    ## 63           telephone_moca_complete.factor                  
    ## 64                               Incomplete      1051 (96.4%)
    ## 65                               Unverified            0 (0%)
    ## 66                                 Complete         39 (3.6%)

### Randomization, Intervention & Control Group Tracking

How randomization of CI is going?

Screening: 39 subjects completed randomization

    ##                                       Overall
    ## 1                                    (N=1090)
    ## 2  randomization_complete.factor             
    ## 3                     Incomplete 1051 (96.4%)
    ## 4                     Unverified       0 (0%)
    ## 5                       Complete    39 (3.6%)
    ## 6               condition.factor             
    ## 7                   Intervention    19 (1.7%)
    ## 8                        Control    20 (1.8%)
    ## 9                        Missing 1051 (96.4%)
    ## 10         intvisit_sched.factor             
    ## 11           Boulder 1.A and 1.B     8 (0.7%)
    ## 12           Boulder 2.A and 2.B     7 (0.6%)
    ## 13           Boulder 3.A and 3.B     3 (0.3%)
    ## 14                           TBD       0 (0%)
    ## 15             Not yet scheduled     1 (0.1%)
    ## 16                       Missing 1071 (98.3%)

Baseline: 37 subjects in total - 31 subjects have cogstat, 6 missing

    ##                     Overall
    ## 1                    (N=37)
    ## 2 cogstat.factor           
    ## 3              1  7 (18.9%)
    ## 4              2 20 (54.1%)
    ## 5              3  4 (10.8%)
    ## 6        Missing  6 (16.2%)

Distribution of cogstat among the 39 subjects who completed
randomization:

    ##                     Overall
    ## 1                    (N=39)
    ## 2 cogstat.factor           
    ## 3              1  7 (17.9%)
    ## 4              2 20 (51.3%)
    ## 5              3  4 (10.3%)
    ## 6        Missing  8 (20.5%)

Distribution of cogstat among the 39 subjects who completed
randomization by condition.factor:

    ##                  Intervention    Control    Overall
    ## 1                      (N=19)     (N=20)     (N=39)
    ## 2 cogstat.factor                                   
    ## 3              1    5 (26.3%)  2 (10.0%)  7 (17.9%)
    ## 4              2    9 (47.4%) 11 (55.0%) 20 (51.3%)
    ## 5              3     1 (5.3%)  3 (15.0%)  4 (10.3%)
    ## 6        Missing    4 (21.1%)  4 (20.0%)  8 (20.5%)
