# SDP-WPHD
# References of Datasets
1. Tantithamthavorn, C., McIntosh, S., Hassan, A.E., Ihara, A., Matsumoto, K. (2015). The impact of mislabelling on the performance and interpretation of defect prediction models. In: 2015 IEEE/ACM 37th IEEE International Conference on Software Engineering, Vol. 1, pp. 812–823. IEEE.

2. Shepperd, M., Song, Q., Sun, Z., & Mair, C. (2013). Data quality: Some comments on the NASA software defect datasets. IEEE Transactions on Software Engineering, 39(9), 1208–1215.

3. Wu, R., Zhang, H., Kim, S., & Cheung, S.-C. (2011). ReLink: Recovering links between bugs and changes. In: Proceedings of the 19th ACM SIGSOFT Symposium and the 13th European Conference on Foundations of Software Engineering, pp. 15–25.

4. D’Ambros, M., Lanza, M., & Robbes, R. (2010). An extensive comparison of bug prediction approaches. In: 2010 7th IEEE Working Conference on Mining Software Repositories (MSR 2010), pp. 31–41. IEEE.

5. Yatish, S., Jiarpakdee, J., Thongtanunam, P., & Tantithamthavorn, C. (2019). Mining software defects: Should we consider affected releases? In: 2019 IEEE/ACM 41st International Conference on Software Engineering (ICSE), pp. 654–665. IEEE.

6. Menzies, T., Krishna, R., & Pryor, D. (2015). The PROMISE repository of empirical software engineering data. Available at: http://promisedata.googlecode.com


# Metrics Details of Softlab
| **Metric**                         | **Description**                                                                |
| ---------------------------------- | ------------------------------------------------------------------------------ |
| `total_loc`                        | Total lines of code (including all types of lines: blank, comment, executable) |
| `blank_loc`                        | Blank lines within the software module                                         |
| `comment_loc`                      | Number of lines containing comments                                            |
| `code_and_comment_loc`             | Total of lines containing either code or comments                              |
| `executable_loc`                   | Number of lines that contain executable statements                             |
| `unique_operands`                  | Count of distinct operands (Halstead metric)                                   |
| `unique_operators`                 | Count of distinct operators (Halstead metric)                                  |
| `total_operands`                   | Total occurrences of operands                                                  |
| `total_operators`                  | Total occurrences of operators                                                 |
| `halstead_vocabulary`              | Number of unique operators and operands (n1 + n2)                              |
| `halstead_length`                  | Total number of operators and operands (N1 + N2)                               |
| `halstead_volume`                  | Volume = Length × log₂(Vocabulary)                                             |
| `halstead_level`                   | Level = 2 × (unique\_operators / (unique\_operands × total\_operators))        |
| `halstead_difficulty`              | Difficulty = (unique\_operators / 2) × (total\_operands / unique\_operands)    |
| `halstead_effort`                  | Effort = Volume × Difficulty                                                   |
| `halstead_error`                   | Estimated number of errors (Volume / 3000)                                     |
| `halstead_time`                    | Programming time = Effort / 18 seconds                                         |
| `branch_count`                     | Number of branches in the control flow                                         |
| `decision_count`                   | Number of decision points (e.g., if/else, switch, etc.)                        |
| `call_pairs`                       | Number of function/method calls                                                |
| `condition_count`                  | Number of conditional expressions                                              |
| `multiple_condition_count`         | Number of conditions involving compound expressions                            |
| `cyclomatic_complexity`            | McCabe’s metric: number of independent paths through code                      |
| `cyclomatic_density`               | Cyclomatic complexity normalized by total LOC or decisions                     |
| `decision_density`                 | Ratio of decision points to total LOC                                          |
| `design_complexity`                | Interval complexity (reflecting structural design choices)                     |
| `design_density`                   | Ratio of design complexity to LOC                                              |
| `normalized_cyclomatic_complexity` | Cyclomatic complexity scaled by other complexity factors                       |
| `formal_parameters`                | Number of formal parameters declared in module/function headers                |


# Metrics Details of NASA
| **Metric**                        | **Description**                                                          |
| --------------------------------- | ------------------------------------------------------------------------ |
| `LOC_BLANK`                       | Number of blank lines in the module                                      |
| `BRANCH_COUNT`                    | Total number of branches in the module                                   |
| `CALL_PAIRS`                      | Number of function call pairs                                            |
| `LOC_CODE_AND_COMMENT`            | Lines of code including comments                                         |
| `LOC_COMMENTS`                    | Number of comment lines                                                  |
| `CONDITION_COUNT`                 | Total number of conditions (e.g., `if`, `while`, etc.)                   |
| `CYCLOMATIC_COMPLEXITY`           | Standard cyclomatic complexity (McCabe’s metric)                         |
| `CYCLOMATIC_DENSITY`              | Cyclomatic complexity normalized by logical lines                        |
| `DECISION_COUNT`                  | Number of decision points (branches)                                     |
| `DECISION_DENSITY`                | Ratio of decision points to total LOC                                    |
| `DESIGN_COMPLEXITY`               | Design complexity, often equal to McCabe’s interval complexity           |
| `DESIGN_DENSITY`                  | Ratio of design complexity to LOC                                        |
| `EDGE_COUNT`                      | Number of edges in the control flow graph                                |
| `ESSENTIAL_COMPLEXITY`            | Measure of structuredness; minimum cycles needed                         |
| `ESSENTIAL_DENSITY`               | Essential complexity relative to LOC                                     |
| `LOC_EXECUTABLE`                  | Lines of executable code                                                 |
| `PARAMETER_COUNT`                 | Number of parameters for functions or methods                            |
| `GLOBAL_DATA_COMPLEXITY`          | Complexity due to global data usage                                      |
| `GLOBAL_DATA_DENSITY`             | Global data complexity relative to LOC                                   |
| `HALSTEAD_CONTENT`                | Halstead content metric (information content)                            |
| `HALSTEAD_DIFFICULTY`             | Halstead difficulty metric                                               |
| `HALSTEAD_EFFORT`                 | Halstead effort metric                                                   |
| `HALSTEAD_ERROR_EST`              | Estimated number of errors (Halstead-based)                              |
| `HALSTEAD_LENGTH`                 | Total number of operators and operands                                   |
| `HALSTEAD_LEVEL`                  | Program level (Halstead metric)                                          |
| `HALSTEAD_PROG_TIME`              | Estimated programming time (Halstead)                                    |
| `HALSTEAD_VOLUME`                 | Program volume (Halstead)                                                |
| `MAINTENANCE_SEVERITY`            | Severity or cost of maintaining the module                               |
| `MODIFIED_CONDITION_COUNT`        | Number of modified condition/decision constructs (MC/DC)                 |
| `MULTIPLE_CONDITION_COUNT`        | Number of conditions with multiple decision clauses                      |
| `NODE_COUNT`                      | Number of nodes in the control flow graph                                |
| `NORMALIZED_CYLOMATIC_COMPLEXITY` | Cyclomatic complexity normalized by decision density                     |
| `NUM_OPERANDS`                    | Total number of operands                                                 |
| `NUM_OPERATORS`                   | Total number of operators                                                |
| `NUM_UNIQUE_OPERANDS`             | Number of unique operands                                                |
| `NUM_UNIQUE_OPERATORS`            | Number of unique operators                                               |
| `NUMBER_OF_LINES`                 | Total number of lines in the module                                      |
| `PATHOLOGICAL_COMPLEXITY`         | Degree of unstructured code (often related to `goto` or complex nesting) |
| `PERCENT_COMMENTS`                | Percentage of comment lines relative to total LOC                        |
| `LOC_TOTAL`                       | Total lines including code, comments, and blank lines                    |


# Metrics Details of ReLink 
| **Abbreviation**      | **Description**                                                |
| --------------------- | -------------------------------------------------------------- |
| AvgCyclomatic         | Average Cyclomatic Complexity                                  |
| AvgCyclomaticModified | Average Modified Cyclomatic Complexity                         |
| AvgCyclomaticStrict   | Average Strict Cyclomatic Complexity                           |
| AvgEssential          | Average Essential Complexity                                   |
| AvgLine               | Average Lines                                                  |
| AvgLineBlank          | Average Blank Lines                                            |
| AvgLineCode           | Average Code Lines                                             |
| AvgLineComment        | Average Comment Lines                                          |
| CountLine             | Number of Lines                                                |
| CountLineBlank        | Number of Blank Lines                                          |
| CountLineCode         | Number of Code Lines                                           |
| CountLineCodeDecl     | Number of Declarative Code Lines                               |
| CountLineCodeExe      | Number of Executable Code Lines                                |
| CountLineComment      | Number of Comment Lines                                        |
| CountSemicolon        | Number of Semicolons                                           |
| CountStmt             | Number of Statements                                           |
| CountStmtDecl         | Number of Declarative Statements                               |
| CountStmtExe          | Number of Executive Statements                                 |
| MaxCyclomatic         | Maximum Cyclomatic Complexity of all nested functions          |
| MaxCyclomaticModified | Maximum Modified Cyclomatic Complexity of all nested functions |
| MaxCyclomaticStrict   | Maximum Strict Cyclomatic Complexity of all nested functions   |
| RatioCommentToCode    | Ratio of Comment Lines to Code Lines                           |
| SumCyclomatic         | Sum of Cyclomatic Complexity of all nested functions           |
| SumCyclomaticModified | Sum of Modified Cyclomatic Complexity of all nested functions  |
| SumCyclomaticStrict   | Sum of Strict Cyclomatic Complexity of all nested functions    |
| SumEssential          | Sum of Essential Complexity of all nested functions            |

# Metrics Details of AEEEM 
| **Abbreviation**                   | **Description**                                                                    |
| ---------------------------------- | ---------------------------------------------------------------------------------- |
| ck\_oo\_wmc                        | Weighted method count                                                              |
| ck\_oo\_dit                        | Depth of inheritance tree                                                          |
| ck\_oo\_rfc                        | Response for class                                                                 |
| ck\_oo\_noc                        | Number of children                                                                 |
| ck\_oo\_cbo                        | Coupling between objects                                                           |
| ck\_oo\_lcom                       | Lack of cohesion in methods                                                        |
| ck\_oo\_fanin                      | Number of other classes that reference the class                                   |
| ck\_oo\_fanout                     | Number of other classes referenced by the class                                    |
| ck\_oo\_noa                        | Number of attributes                                                               |
| ck\_oo\_nopa                       | Number of public attributes                                                        |
| ck\_oo\_nopra                      | Number of private attributes                                                       |
| ck\_oo\_noai                       | Number of attributes inherited                                                     |
| ck\_oo\_loc                        | Number of lines of code                                                            |
| ck\_oo\_nom                        | Number of methods                                                                  |
| ck\_oo\_nopm                       | Number of public methods                                                           |
| ck\_oo\_noprm                      | Number of private methods                                                          |
| ck\_oo\_nomt                       | Number of methods inherited                                                        |
| WCHU\_wmc                          | Weighted churn of weighted method count                                            |
| WCHU\_dit                          | Weighted churn of depth of inheritance tree                                        |
| WCHU\_rfc                          | Weighted churn of response for class                                               |
| WCHU\_noc                          | Weighted churn of number of children                                               |
| WCHU\_cbo                          | Weighted churn of coupling between objects                                         |
| WCHU\_lcom                         | Weighted churn of lack of cohesion in methods                                      |
| WCHU\_fanin                        | Weighted churn of number of other classes that reference the class                 |
| WCHU\_fanout                       | Weighted churn of number of other classes referenced by the class                  |
| WCHU\_noa                          | Weighted churn of number of attributes                                             |
| WCHU\_nopa                         | Weighted churn of number of public attributes                                      |
| WCHU\_nopra                        | Weighted churn of number of private attributes                                     |
| WCHU\_noai                         | Weighted churn of number of attributes inherited                                   |
| WCHU\_loc                          | Weighted churn of number of lines of code                                          |
| WCHU\_nom                          | Weighted churn of number of methods                                                |
| WCHU\_nopm                         | Weighted churn of number of public methods                                         |
| WCHU\_noprm                        | Weighted churn of number of private methods                                        |
| WCHU\_nomt                         | Weighted churn of number of methods inherited                                      |
| LDHH\_wmc                          | Linear decayed history entropy of weighted method count                            |
| LDHH\_dit                          | Linear decayed history entropy of depth of inheritance tree                        |
| LDHH\_rfc                          | Linear decayed history entropy of response for class                               |
| LDHH\_noc                          | Linear decayed history entropy of number of children                               |
| LDHH\_cbo                          | Linear decayed history entropy of coupling between objects                         |
| LDHH\_lcom                         | Linear decayed history entropy of lack of cohesion in methods                      |
| LDHH\_fanin                        | Linear decayed history entropy of number of other classes that reference the class |
| LDHH\_fanout                       | Linear decayed history entropy of number of other classes referenced by the class  |
| LDHH\_noa                          | Linear decayed history entropy of number of attributes                             |
| LDHH\_nopa                         | Linear decayed history entropy of number of public attributes                      |
| LDHH\_nopra                        | Linear decayed history entropy of number of private attributes                     |
| LDHH\_noai                         | Linear decayed history entropy of number of attributes inherited                   |
| LDHH\_loc                          | Linear decayed history entropy of number of lines of code                          |
| LDHH\_nom                          | Linear decayed history entropy of number of methods                                |
| LDHH\_nopm                         | Linear decayed history entropy of number of public methods                         |
| LDHH\_noprm                        | Linear decayed history entropy of number of private methods                        |
| LDHH\_nomt                         | Linear decayed history entropy of number of methods inherited                      |
| CvsEntropy                         | Entropy of CVS change log                                                          |
| CvsWEntropy                        | Weighted Entropy of CVS change log                                                 |
| CvsLogEntropy                      | Logarithmic Entropy of CVS change log                                              |
| CvsExpEntropy                      | Exponential Entropy of CVS change log                                              |
| CvsLinEntropy                      | Linear Entropy of CVS change log                                                   |
| numberOfNonTrivialBugsFoundUntil   | Number of non-trivial bugs found until the corresponding fix                       |
| numberOfCriticalBugsFoundUntil     | Number of critical bugs found until the corresponding fix                          |
| numberOfHighPriorityBugsFoundUntil | Number of high priority bugs found until the corresponding fix                     |
| numberOfMajorBugsFoundUntil        | Number of major bugs found until the corresponding fix                             |
| numberOfBugsFoundUntil             | Number of bugs found until the corresponding fix                                   |

# Metrics Details of JIRA 
| **Abbreviation**          | **Description**                                                            |
| ------------------------- | -------------------------------------------------------------------------- |
| AvgCyclomatic             | Average cyclomatic complexity for all nested functions or methods          |
| SumCyclomatic             | Sum of cyclomatic complexity of all nested functions or methods            |
| AvgCyclomaticModified     | Average modified cyclomatic complexity for all nested functions or methods |
| SumCyclomaticModified     | Sum of modified cyclomatic complexity of all nested functions              |
| AvgCyclomaticStrict       | Average strict cyclomatic complexity for all nested functions or methods   |
| SumCyclomaticStrict       | Sum of strict cyclomatic complexity of all nested functions or methods     |
| AvgEssential              | Average essential complexity for all nested functions or methods           |
| SumEssential              | Sum of essential complexity of all nested functions or methods             |
| AvgLine                   | Average number of lines for all nested functions or methods                |
| AvgLineBlank              | Average number of blank lines for all nested functions or methods          |
| AvgLineCode               | Average number of lines containing source code for all nested functions    |
| AvgLineComment            | Average number of comment lines for all nested functions or methods        |
| CountClassBase            | Number of immediate base classes                                           |
| CountClassCoupled         | Number of other classes coupled to                                         |
| CountClassDerived         | Number of immediate subclasses                                             |
| MaxInheritanceTree        | Maximum depth of class in inheritance tree                                 |
| PercentLackOfCohesion     | 100% minus the average cohesion for package entities                       |
| CountDeclClass            | Number of classes                                                          |
| CountDeclClassMethod      | Number of class methods                                                    |
| CountDeclClassVariable    | Number of class variables                                                  |
| CountDeclFunction         | Number of functions                                                        |
| CountDeclInstanceMethod   | Number of instance methods                                                 |
| CountDeclInstanceVariable | Number of instance variables                                               |
| CountDeclMethod           | Number of local (non-inherited) methods                                    |
| CountDeclMethodDefault    | Number of local default methods                                            |
| CountDeclMethodPrivate    | Number of local (non-inherited) private methods                            |
| CountDeclMethodProtected  | Number of local protected methods                                          |
| CountDeclMethodPublic     | Number of local (non-inherited) public methods                             |
| CountLine                 | Number of physical lines                                                   |
| CountLineBlank            | Number of blank lines                                                      |
| CountLineCode             | Number of lines containing source code                                     |
| CountLineCodeDecl         | Number of lines containing declarative source code                         |
| CountLineCodeExe          | Number of lines containing executable source code                          |
| CountLineComment          | Number of lines containing comment                                         |
| CountSemicolon            | Number of semicolons                                                       |
| CountStmt                 | Number of statements                                                       |
| CountStmtDecl             | Number of declarative statements                                           |
| CountStmtExe              | Number of executable statements                                            |
| MaxCyclomatic             | Maximum cyclomatic complexity of all nested functions or methods           |
| MaxCyclomaticModified     | Maximum modified cyclomatic complexity of nested functions or methods      |
| MaxCyclomaticStrict       | Maximum strict cyclomatic complexity of nested functions or methods        |
| RatioCommentToCode        | Ratio of comment lines to code lines                                       |
| CountInput\_Min           | Min number of calling subprograms plus global variables read               |
| CountInput\_Mean          | Mean number of calling subprograms plus global variables read              |
| CountInput\_Max           | Max number of calling subprograms plus global variables read               |
| CountOutput\_Min          | Min number of called subprograms plus global variables set                 |
| CountOutput\_Mean         | Mean number of called subprograms plus global variables set                |
| CountOutput\_Max          | Max number of called subprograms plus global variables set                 |
| CountPath\_Min            | Min number of unique paths through a body of code                          |
| CountPath\_Mean           | Mean number of unique paths through a body of code                         |
| CountPath\_Max            | Max number of unique paths through a body of code                          |
| MaxNesting\_Min           | Min of maximum nesting level of control constructs in the function         |
| MaxNesting\_Mean          | Mean of maximum nesting level of control constructs in the function        |
| MaxNesting\_Max           | Max of maximum nesting level of control constructs in the function         |
| COMM                      | Number of Git commits                                                      |
| ADDED\_LINES              | Normalized number of lines added to the module                             |
| DEL\_LINES                | Normalized number of lines deleted from the module                         |
| ADEV                      | Number of active developers                                                |
| DDEV                      | Number of distinct developers                                              |
| MINOR\_COMMIT             | Developers contributing <5% of total code changes                          |
| MINOR\_LINE               | Developers contributing <5% of total LOC                                   |
| MAJOR\_COMMIT             | Developers contributing >5% of total code changes                          |
| MAJOR\_LINES              | Developers contributing >5% of total LOC                                   |
| OWN\_COMMIT               | Proportion of code changes by top contributor                              |
| OWN\_LINE                 | Proportion of lines of code by top contributor                             |

# Metrics Details of PROMISE
| **Abbreviation** | **Description** |
|------------------|-----------------|
| WMC              | Weighted Methods per Class |
| DIT              | Depth of Inheritance Tree |
| NOC              | Number of Children |
| CBO              | Coupling Between Object Classes |
| RFC              | Response for a Class |
| LCOM             | Lack of Cohesion in Methods |
| CA               | Afferent Couplings |
| CE               | Efferent Couplings |
| NPM              | Number of Public Methods |
| LCOM3            | Lack of Cohesion in Methods (variant of LCOM) |
| LOC              | Lines of Code |
| DAM              | Data Access Metric |
| MOA              | Measure of Aggregation |
| MFA              | Measure of Functional Abstraction |
| CAM              | Cohesion Among Methods of a Class |
| IC               | Inheritance Coupling |
| CBM              | Coupling Between Methods |
| AMC              | Average Method Complexity |
| CC               | McCabe’s Cyclomatic Complexity |
| MAX_CC           | Maximum Value of CC Among Methods in the Class |
| AVG_CC           | Average (Arithmetic Mean) CC of Methods in the Class |
