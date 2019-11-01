# Mongo-Chat

##Lab 9, DS

'''bash 
{
        "_id" : "rs0",
        "version" : 1,
        "protocolVersion" : NumberLong(1),
        "writeConcernMajorityJournalDefault" : true,
        "members" : [
                {
                        "_id" : 0,
                        "host" : "mongofirst:27017",
                        "arbiterOnly" : false,
                        "buildIndexes" : true,
                        "hidden" : false,
                        "priority" : 1,
                        "tags" : {

                        },
                        "slaveDelay" : NumberLong(0),
                        "votes" : 1
                },
                {
                        "_id" : 1,
                        "host" : "mongosecond:27017",
                        "arbiterOnly" : false,
                        "buildIndexes" : true,
                        "hidden" : false,
                        "priority" : 1,
                        "tags" : {

                        },
                        "slaveDelay" : NumberLong(0),
                        "votes" : 1
                },
                {
                        "_id" : 2,
                        "host" : "mongothird:27017",
                        "arbiterOnly" : false,
                        "buildIndexes" : true,
                        "hidden" : false,
                        "priority" : 1,
                        "tags" : {

                        },
                        "slaveDelay" : NumberLong(0),
                        "votes" : 1
                }
        ],
        "settings" : {
                "chainingAllowed" : true,
                "heartbeatIntervalMillis" : 2000,
                "heartbeatTimeoutSecs" : 10,
                "electionTimeoutMillis" : 10000,
                "catchUpTimeoutMillis" : -1,
                "catchUpTakeoverDelayMillis" : 30000,
                "getLastErrorModes" : {

                },
                "getLastErrorDefaults" : {
                        "w" : 1,
                        "wtimeout" : 0
                },
                "replicaSetId" : ObjectId("6fdf486a5iwe987e1fs5s48e")
        }
}
'''

'''bash
{
        "set" : "rs0",
        "date" : ISODate("2019-11-01T20:50:26.219Z"),
        "myState" : 2,
        "term" : NumberLong(3),
        "syncingTo" : "",
        "syncSourceHost" : "",
        "syncSourceId" : -1,
        "heartbeatIntervalMillis" : NumberLong(2000),
        "majorityVoteCount" : 2,
        "writeMajorityCount" : 2,
        "optimes" : {
                "lastCommittedOpTime" : {
                        "ts" : Timestamp(1572635320, 1),
                        "t" : NumberLong(2)
                },
                "lastCommittedWallTime" : ISODate("2019-11-01T20:48:40.221Z"),
                "readConcernMajorityOpTime" : {
                        "ts" : Timestamp(1572635320, 1),
                        "t" : NumberLong(2)
                },
                "readConcernMajorityWallTime" : ISODate("2019-11-01T20:48:40.221Z"),
                "appliedOpTime" : {
                        "ts" : Timestamp(1572635320, 1),
                        "t" : NumberLong(2)
                },
                "durableOpTime" : {
                        "ts" : Timestamp(1572635320, 1),
                        "t" : NumberLong(2)
                },
                "lastAppliedWallTime" : ISODate("2019-11-01T20:48:40.221Z"),
                "lastDurableWallTime" : ISODate("2019-11-01T20:48:40.221Z")
        },
        "lastStableRecoveryTimestamp" : Timestamp(1572635320, 1),
        "lastStableCheckpointTimestamp" : Timestamp(1572635320, 1),
        "electionCandidateMetrics" : {
                "lastElectionReason" : "electionTimeout",
                "lastElectionDate" : ISODate("2019-11-01T20:44:14.667Z"),
                "termAtElection" : NumberLong(1),
                "lastCommittedOpTimeAtElection" : {
                        "ts" : Timestamp(0, 0),
                        "t" : NumberLong(-1)
                },
                "lastSeenOpTimeAtElection" : {
                        "ts" : Timestamp(1572478684, 1),
                        "t" : NumberLong(-1)
                },
                "numVotesNeeded" : 2,
                "priorityAtElection" : 1,
                "electionTimeoutMillis" : NumberLong(10000),
                "numCatchUpOps" : NumberLong(27017),
                "newTermStartDate" : ISODate("2019-11-01T20:44:15.301Z"),
                "wMajorityWriteAvailabilityDate" : ISODate("2019-11-01T20:44:15.977Z")
        },
        "members" : [
                {
                        "_id" : 0,
                        "name" : "mongofirst:27017",
                        "ip" : "127.31.6.9",
                        "health" : 1,
                        "state" : 1,
                        "stateStr" : "PRIMARY",
                        "uptime" : 4543,
                        "optime" : {
                                "ts" : Timestamp(1572483120, 1),
                                "t" : NumberLong(1)
                        },
                        "optimeDate" : ISODate("2019-11-01T21:58:05Z"),
                        "syncingTo" : "",
                        "syncSourceHost" : "",
                        "syncSourceId" : -1,
                        "infoMessage" : "",
                        "electionTime" : Timestamp(1572478694, 1),
                        "electionDate" : ISODate("2019-11-01T20:44:14Z"),
                        "configVersion" : 1,
                        "self" : true,
                        "lastHeartbeatMessage" : ""
                },
                {
                        "_id" : 1,
                        "name" : "mongosecond:27017",
                        "ip" : "172.31.29.4",
                        "health" : 1,
                        "state" : 2,
                        "stateStr" : "SECONDARY",
                        "uptime" : 4442,
                        "optime" : {
                                "ts" : Timestamp(1572483120, 1),
                                "t" : NumberLong(1)
                        },
                        "optimeDurable" : {
                                "ts" : Timestamp(1572483120, 1),
                                "t" : NumberLong(1)
                        },
                        "optimeDate" : ISODate("2019-11-01T21:58:05Z"),
                        "optimeDurableDate" : ISODate("2019-11-01T21:58:05Z"),
                        "lastHeartbeat" : ISODate("2019-11-01T21:58:06.870Z"),
                        "lastHeartbeatRecv" : ISODate("2019-11-01T21:58:06.146Z"),
                        "pingMs" : NumberLong(0),
                        "lastHeartbeatMessage" : "",
                        "syncingTo" : "mongofirst:27017",
                        "syncSourceHost" : "mongofirst:27017",
                        "syncSourceId" : 0,
                        "infoMessage" : "",
                        "configVersion" : 1
                },
                {
                        "_id" : 2,
                        "name" : "mongothird:27017",
                        "ip" : "172.31.22.105",
                        "health" : 1,
                        "state" : 2,
                        "stateStr" : "SECONDARY",
                        "uptime" : 4442,
                        "optime" : {
                                "ts" : Timestamp(1572483115, 1),
                                "t" : NumberLong(1)
                        },
                        "optimeDurable" : {
                                "ts" : Timestamp(1572483115, 1),
                                "t" : NumberLong(1)
                        },
                        "optimeDate" : ISODate("2019-11-01T21:58:55Z"),
                        "optimeDurableDate" : ISODate("2019-11-01T21:58:55Z"),
                        "lastHeartbeat" : ISODate("2019-11-01T21:58:04.969Z"),
                        "lastHeartbeatRecv" : ISODate("2019-11-01T21:58:06.277Z"),
                        "pingMs" : NumberLong(1),
                        "lastHeartbeatMessage" : "",
                        "syncingTo" : "mongofirst:27017",
                        "syncSourceHost" : "mongofirst:27017",
                        "syncSourceId" : 0,
                        "infoMessage" : "",
                        "configVersion" : 1
                }
        ],
        "ok" : 1,
        "$clusterTime" : {
                "clusterTime" : Timestamp(1572483120, 1),
                "signature" : {
                        "hash" : BinData(0,"AAAAAAAAAAAAAAAAAAAAAAAAAAA="),
                        "keyId" : NumberLong(0)
                }
        },
        "operationTime" : Timestamp(1572483120, 1)
}
'''
