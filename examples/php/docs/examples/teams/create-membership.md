<?php

use Appwrite\Client;
use Appwrite\Services\Teams;

$client = new Client();

$client
    ->setProject('')
;

$teams = new Teams($client);

$result = $teams->createMembership('[TEAM_ID]', 'email@example.com', [], 'https://example.com');