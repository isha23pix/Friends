<template>
    <v-container fluid>
       <v-list>
        <v-card @click="openChat(chat)" v-for="chat in chats" :key="chat.id" two-line>
            <v-card-actions>
          <v-row no-gutters align="center">

            <!-- Avatar Column -->
            <v-col cols="2">
              <v-avatar>
                <img :src="chat.profileImage" alt="Profile image">
              </v-avatar>
            </v-col>

            <!-- Name and Message Column -->
            <v-col cols="4">
              <v-list-item-content>
                <v-list-item-title>{{ chat.name }}</v-list-item-title>
                <v-list-item-subtitle>{{ chat.lastMessage }}</v-list-item-subtitle>
              </v-list-item-content>
            </v-col>

            <!-- Seen/Unseen Icon and Time -->
            <v-col cols="4">
              <v-row justify="end">
                <div class="justify-self-end">
                <v-list-item-action class="me-1">
                  <div v-if="chat.unreadCount > 0">
                    <v-badge color="#6e00ff" :content="chat.unreadCount">
                      <v-icon color="grey">mdi-message</v-icon>
                    </v-badge>
                  </div>
                  <!-- <div v-else>
                    <v-icon :color="chat.seen ? '6e00ff' : 'default'">
                      {{ chat.seen ? 'mdi-check-all' : 'mdi-check' }}
                    </v-icon>
                  </div> -->
                </v-list-item-action> 
                <!-- <v-list-item-action-text class="custom-time">{{ chat.time }}</v-list-item-action-text> -->
              </div>
              </v-row>
            </v-col>

          </v-row>
        </v-card-actions>
            
        </v-card>
       </v-list>
   </v-container>
 </template>
 
 <script>
     export default {
         name:"ChatList",
         data() {
         return {
         chats: [
         {
           id: 1,
           name: 'Alice Freeman',
           lastMessage: 'Hey, how’s it going?',
           profileImage: 'https://static.vecteezy.com/system/resources/previews/002/275/847/original/male-avatar-profile-icon-of-smiling-caucasian-man-vector.jpg',
           time: '15 min ago',
           seen: true,
           unreadCount: 0,
         },
         {
           id: 2,
           name: 'Claire Blue',
           lastMessage: 'Hey, Pay me!',
           profileImage: 'https://e7.pngegg.com/pngimages/799/987/png-clipart-computer-icons-avatar-icon-design-avatar-heroes-computer-wallpaper-thumbnail.png',
           time: '45 min ago',
           seen: false,
           unreadCount: 0,
         },
         {
           id: 3,
           name: 'Daisy Ros',
           lastMessage: 'Hey, what is up?',
           profileImage: 'https://www.svgrepo.com/show/382100/female-avatar-girl-face-woman-user-7.svg',
           time: '35 min ago',
           seen: false,
           unreadCount: 5,
         },
       ]
     };
   }
     }
 </script>
 
 <style scoped>
 .v-container{
    border-radius: 5px;
 }
 .v-list-item {
  margin-bottom: 8px;
}

::v-deep .v-avatar img {
  border-radius: 50%; /* Makes the image round */
  width: 40px; /* Controls the width of the image */
  height: 40px; /* Controls the height of the image */
}

.v-list-item-action-text {
  margin-right: 10px;
}

.v-card {
  background-color: #ffffff;
  padding-top: 8px;
}

 .v-list-item {
  align-items: center; /* Ensures vertical alignment is centered */
}


.custom-time {
  color: #555; /* Change the color of the time text */
}

 </style>