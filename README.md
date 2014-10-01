<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <title>Rabbit MQ Monitor Plugin</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
    <meta http-equiv="X-UA-Compatible" content="IE=EmulateIE8" />
    <meta content="Scroll Wiki Publisher" name="generator"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/liquid.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/print.css" media="print"/>
    <link type="text/css" rel="stylesheet" href="css/content-style.css" media="screen, projection, print"/>
    <link type="text/css" rel="stylesheet" href="css/screen.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/print.css" media="print"/>
</head>
<body>
                <h1>Rabbit MQ Monitor Plugin</h1>
    <p>
<a href="attachments_163546851_1_com.RabbitMQ.RabbitMQMonitor_1.2.0.jar">Rabbit MQ Monitoring Plugin 1.2</a>    </p>
    <p>
    </p>
    <p>
            <img src="images_community/download/attachments/119079240/icon.png" alt="images_community/download/attachments/119079240/icon.png" class="confluence-embedded-image image-left" />
        The monitor returns a number of values associated with RabbitMQ. The RabbitMQ Monitor makes 2 initial calls to the RabbitMQ rest interface which gets the overview and node information.    </p>
    <p>
The plug-in then uses the JSon-simple library to parse the JSon script returned from the rest interface into an overview and nodes object. The overview object contains the values from the overview of the RabbitMQ Server. The Nodes object contains an array of Node objects. One Node object is created for each node returned in the JSon script. The Node is used to hold information about individual nodes.    </p>
    <p>
Finally the monitor iterates through the measures and uses the correct objects to match each measure. If a Node measure is created the Node Name is a required field in the Measure configuration. This will tell the Nodes object which Node to pull the information from. If a Queue Measure is created the monitor will make an additional call to the RabbitMQ rest interface to retrieve data about the Queue specified in the measure configuration.    </p>
    <p>
    </p>
    <div class="tablewrap">
        <table>
<thead class=" "></thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/119079240/t1.jpg" alt="images_community/download/attachments/119079240/t1.jpg" class="" />
            </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/119079240/RabbitMQ.jpg" alt="images_community/download/attachments/119079240/RabbitMQ.jpg" class="" />
            </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/119079240/RabbitMQ_Monitor.jpg" alt="images_community/download/attachments/119079240/RabbitMQ_Monitor.jpg" class="" />
            </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
                </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/119079240/RabbitMQ_Measures.jpg" alt="images_community/download/attachments/119079240/RabbitMQ_Measures.jpg" class="" />
            </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/119079240/RabbitMQ_Measures_Queue_Properties.jpg" alt="images_community/download/attachments/119079240/RabbitMQ_Measures_Queue_Properties.jpg" class="" />
            </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/119079240/RabbitMQ_Measure_Node_Properties.jpg" alt="images_community/download/attachments/119079240/RabbitMQ_Measure_Node_Properties.jpg" class="" />
            </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
                </td>
        </tr>
</tbody>        </table>
            </div>
    <div class="section-2"  id="119079240_RabbitMQMonitorPlugin-PluginDetails"  >
        <h2>Plugin Details</h2>
    <div class="tablewrap">
        <table>
<thead class=" "></thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Plug-In Versions    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_163546851_1_com.RabbitMQ.RabbitMQMonitor_1.2.0.jar">Rabbit MQ Monitoring Plugin</a> (compatible with dynaTrace 4.x)<br/><a href="attachments_119373869_1_RabbitMQ.dashboard.xml">Rabbit MQ Dashboard</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Author    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Derek Abing    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
License    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_5275722_2_dynaTraceBSD.txt">dynaTrace BSD</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Support    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="https://community/display/DL/Support+Levels#SupportLevels-Community">Not Supported </a><br/>If you have any questions or suggestions for these plugins, please add a comment to this page, use our <a href="https://community.dynatrace.com/community/pages/viewpage.action?pageId=46628918">forum</a>, or drop us an email at <a href="mailto:community@dynatrace.com">community@dynatrace.com</a>!    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Known Problems    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Release History    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
2012-04-18 Initial Release<br/>2013-09-25 Update    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    </div>
    <div class="section-2"  id="119079240_RabbitMQMonitorPlugin-ProvidedMeasures"  >
        <h2>Provided Measures</h2>
    <div class="tablewrap">
        <table>
<thead class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Measure Name    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Description    </p>
            </td>
        </tr>
</thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Active Consumers    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The number of consumers in the active state for a queue    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Consumers    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The number of consumers in a queue    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Disk Alarm    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Returns a 1 if the disk alarm has been tripped and a 0 if the disk alarm has not been tripped.    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Disk Free    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The amount of free bytes on the disk    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
EventCorrelationEngine.MainSubscription Active Consumers    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The number of consumers in the active state for a queue    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
EventCorrelationEngine.MainSubscription Consumers    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The number of consumers in a queue    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
EventCorrelationEngine.MainSubscription Messages    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The total number of messages in a queue    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
EventingLoadTest.BPClaims_AssignmentClaim Acitve Consumers    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The number of consumers in the active state for a queue    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
EventingLoadTest.BPClaims_AssignmentClaim Messages    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The total number of messages in a queue    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Memory Alarm    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Returns a 1 if the memory alarm has been tripped and a 0 if the memory alarm has not been tripped.    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Memory Used    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The amount of bytes used by the Node    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Messages    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The total number of messages in the HornetQ instance.    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Messages Ready    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Total number of messages in the &quot;Ready&quot; state.    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Messages Unacknowledged    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The number of messages in the Unacknowledged state in the queue    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Node Running    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Returns a 1 if the node is running and a 0 if the node is down.    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    </div>
    <div class="section-2"  id="119079240_RabbitMQMonitorPlugin-Configuration"  >
        <h2>Configuration</h2>
    <div class="tablewrap">
        <table>
<thead class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Name    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Value    </p>
            </td>
        </tr>
</thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Rest Port    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Port on the server used by the restful interface.    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Username    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The username to use for authentication to the restful interface    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Password    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The password for the username used to authenticate to the restful interface.    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    </div>
    <div class="section-2"  id="119079240_RabbitMQMonitorPlugin-Installation"  >
        <h2>Installation</h2>
    <p>
Import the Plugin into the dynaTrace Server. For details how to do this please refer to the <a href="https://community.dynatrace.com/community/display/DOCDT50/Manage+and+Develop+User+Plugins">dynaTrace documentation</a>.    </p>
    </div>
            </div>
        </div>
        <div class="footer">
        </div>
    </div>
</body>
</html>
